# AGENTS.md — AI Agent Guidelines for This Repository

This file provides guidance for AI coding agents (GitHub Copilot, Claude, etc.) working on this LaTeX-based software engineering roadmap repository.

---

## 📌 Project Context

- This is a **LaTeX document repository** containing a 25-phase, 108-week software engineering learning roadmap
- The primary file is `roadmap.tex`, which compiles to a PDF via GitHub Actions on every push that modifies it
- The repo also contains `prompt-collection.md` with enhancement prompts designed for use with Perplexity AI Deep Research

---

## 🛠️ Tech Stack

| Component | Details |
|-----------|---------|
| Document engine | LaTeX compiled with `pdflatex` |
| Custom environments | `tcolorbox`, `longtable`, `fancyhdr`, `titlesec`, `hyperref`, `enumitem`, `booktabs`, `xcolor` |
| CI/CD | GitHub Actions using `xu-cheng/latex-action` |
| Hosting | GitHub Pages (PDF served at `https://gkrishna247.github.io/software-engineering-roadmap/roadmap.pdf`) |

---

## 📂 File Structure

| File | Role |
|------|------|
| `roadmap.tex` | **PRIMARY CONTENT FILE** — Main LaTeX source for the full roadmap |
| `prompt-collection.md` | Enhancement prompts for AI research tools (Perplexity AI Deep Research) |
| `.github/workflows/compile-latex.yml` | Auto-compile workflow: LaTeX → PDF → GitHub Pages |
| `README.md` | Project documentation and quick-start guide |

---

## ⌨️ Commands Agents Can Use

```bash
# Validate LaTeX syntax (stops on first error)
pdflatex -interaction=nonstopmode -halt-on-error roadmap.tex

# Check for undefined references after compilation
grep -n "undefined" roadmap.log

# Count chapters and sections (approximate phase count)
grep -c "\\\\chapter\|\\\\section" roadmap.tex
```

---

## 📐 Content Structure Rules

### Six-Part Topic Template
Every topic inside a phase **must** follow this structure:
1. **Prerequisite Concepts** — what the learner needs to know before starting
2. **Core Concepts Deep Explanation** — thorough, precise explanation of the topic
3. **Advanced Trajectory** — where this topic leads and how it connects to later phases
4. **Common Pitfalls and Debugging** — mistakes beginners make and how to avoid them
5. **Cross-Phase Connections** — explicit links to related content in other phases
6. **Hands-On Exercises** — concrete coding tasks to cement understanding

### Phase Structure
Each phase must contain the following LaTeX elements, in order:

| Element | Purpose |
|---------|---------|
| `prereqbox` | Lists prerequisite knowledge for the phase |
| `topics` | Main content sections with the six-part template |
| `microcheckpoint` | Self-assessment questions mid-phase |
| Resource `longtable` | Curated resources table (see column spec below) |
| Books `\begin{itemize}` | Recommended books list |
| `milestonebox` | End-of-phase milestone project |
| `practicebox` | Additional practice exercises |

### Resource Table Columns
All resource `longtable` entries use these exact columns:

| Column | Description |
|--------|-------------|
| Resource | Name and link of the resource |
| Format | e.g., Video, Book, Article, Course |
| Cost | Free / Paid / Freemium |
| Role | Primary / Supplementary / Reference |
| Why Best | One-line justification |
| Produce With It | Concrete output the learner creates |

---

## 🎨 Code Style for LaTeX

- **Use custom `tcolorbox` environments** (`prereqbox`, `milestonebox`, `practicebox`, `microcheckpoint`) — never raw `\begin{tcolorbox}` directly
- **Wrap all URLs** in `\url{}` (plain URLs) or `\href{url}{text}` (linked text) — never bare URLs
- **Use `\paragraph{}`** for topic-level resource headings, not `\subsection{}`
- **Escape special characters** properly: `\&` `\%` `\$` `\#` `\_`
- **Indentation**: 2 spaces inside all environments — keep it consistent
- **No orphaned environments**: always close every `\begin{}` with a matching `\end{}`

---

## 🚦 Boundaries

### ✅ ALWAYS
- Preserve existing LaTeX formatting and custom environments
- Maintain the six-part topic template for all new content
- Wrap all URLs in `\url{}` or `\href{}`
- Verify the document compiles successfully before marking work complete
- Use conventional commit messages (`feat:`, `fix:`, `docs:`, `chore:`)

### ⚠️ ASK FIRST
- Before restructuring chapters or phases (changing phase order or numbering)
- Before adding new LaTeX packages to the preamble
- Before changing the document class or geometry settings
- Before making bulk find-and-replace changes across the file

### 🚫 NEVER
- Remove existing content — only add or enhance
- Modify the preamble package configuration without an explicit request
- Change visual styling (colors, fonts, spacing, layout)
- Leave unclosed LaTeX environments that would break compilation
- Commit a version that fails `pdflatex -halt-on-error`

---

## ✍️ Writing Style

- **Technical but accessible** — assume the reader is motivated but not yet expert
- **Encouraging but honest** — acknowledge difficulty without being discouraging
- **Every sentence must teach something** — no filler, no padding
- **Precise terminology** — use correct technical terms; add a brief inline explanation on first use of complex terms
- **Consistent tone** — match the register of surrounding phases; do not introduce a markedly different voice

---

## 🔀 Git Workflow

- **Commit message format**: [Conventional Commits](https://www.conventionalcommits.org/) — scopes are optional but encouraged when targeting a specific phase (e.g., `feat(phase-12):`)
  - `feat: add Phase 12 React section with project exercises`
  - `feat(phase-7): expand DSA section with graph algorithms`
  - `fix: correct undefined reference in Phase 7 resource table`
  - `docs: update README quick-start instructions`
  - `chore: clean up auxiliary LaTeX build files`
- **Trigger awareness**: only changes to `roadmap.tex` trigger the compile workflow; changes to other files do not produce a new PDF automatically
- **Compile before pushing**: always run `pdflatex -interaction=nonstopmode -halt-on-error roadmap.tex` locally and confirm it exits with code `0` before pushing
