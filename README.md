# 🗺️ Software Engineering Mastery Roadmap

<div align="center">

[![LaTeX Compile](https://img.shields.io/github/actions/workflow/status/gkrishna247/software-engineering-roadmap/compile-latex.yml?label=LaTeX%20Compile&logo=latex&logoColor=white)](https://github.com/gkrishna247/software-engineering-roadmap/actions/workflows/compile-latex.yml)
[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-blue?logo=github)](https://gkrishna247.github.io/software-engineering-roadmap/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Last Commit](https://img.shields.io/github/last-commit/gkrishna247/software-engineering-roadmap)](https://github.com/gkrishna247/software-engineering-roadmap/commits/main)

**A comprehensive 25-phase, 108-week software engineering mastery roadmap — from fundamentals to industry-ready expertise.**

[📄 View PDF Roadmap](https://gkrishna247.github.io/software-engineering-roadmap/roadmap.pdf) · [🐛 Report an Issue](https://github.com/gkrishna247/software-engineering-roadmap/issues) · [💡 Suggest a Topic](https://github.com/gkrishna247/software-engineering-roadmap/issues/new)

</div>

---

## 📖 Overview

This repository contains a structured, project-based software engineering learning roadmap designed to take you from the absolute basics all the way to professional mastery. Spanning **25 phases** and **108 weeks**, it provides a clear, week-by-week curriculum covering every major area of modern software engineering — including systems programming, algorithms, full-stack web development, AI/ML, DevOps, cloud architecture, and career preparation.

The roadmap is aimed at **self-taught developers** who want a structured path without a formal degree, **CS students** looking to complement their coursework with practical industry skills, and **career switchers** who need a comprehensive guide to break into software engineering. Each phase builds on the previous one, ensuring a solid foundation before advancing to more complex topics.

The learning philosophy is **project-based and consistent**: dedicate approximately **4 hours per day** to hands-on coding and conceptual study. Rather than passive reading, every phase emphasizes building real projects to reinforce concepts. The roadmap progresses through four tiers — Foundation, Core Programming, Professional Skills, and Specialization + Career — each tier unlocking the next level of expertise.

---

## 🏗️ Roadmap Structure

The roadmap is organized into **4 tiers** containing **25 phases** across **108 weeks**:

| Tier | Phases | Weeks | Focus Areas |
|------|--------|-------|-------------|
| **Tier 0 — Foundation** | 1–3 | 1–12 | C Programming, Linux & Shell scripting, Computer Science fundamentals |
| **Tier 1 — Core Programming** | 4–10 | 13–40 | Python, Java, Data Structures & Algorithms, Databases (SQL & NoSQL), Networking, Mathematics for AI |
| **Tier 2 — Professional Skills** | 11–18 | 41–72 | Web Development (HTML/CSS/JS, React, Node.js), Testing & CI/CD, Software Architecture, DevOps & Cloud, Security, Observability & Monitoring |
| **Tier 3 — Specialization + Career** | 19–25 | 73–108 | Machine Learning, Deep Learning, Generative AI & LLMs, Data Engineering, MLOps, Modern Languages (Rust, Go, TypeScript), System Design & Career Preparation |

<details>
<summary><b>📋 Full Phase Breakdown</b></summary>

| Phase | Weeks | Topic |
|-------|-------|-------|
| Phase 1 | 1–4 | C Programming fundamentals |
| Phase 2 | 5–8 | Advanced C & memory management |
| Phase 3 | 9–12 | Linux, shell scripting & CS fundamentals |
| Phase 4 | 13–16 | Python programming |
| Phase 5 | 17–20 | Advanced Python & scripting |
| Phase 6 | 21–24 | Java & object-oriented design |
| Phase 7 | 25–28 | Data Structures & Algorithms (Part 1) |
| Phase 8 | 29–32 | Data Structures & Algorithms (Part 2) |
| Phase 9 | 33–36 | Databases (SQL & NoSQL) |
| Phase 10 | 37–40 | Networking & Mathematics for AI |
| Phase 11 | 41–44 | Web Development fundamentals |
| Phase 12 | 45–48 | Frontend: React & modern JavaScript |
| Phase 13 | 49–52 | Backend: Node.js & REST APIs |
| Phase 14 | 53–56 | Testing strategies & CI/CD pipelines |
| Phase 15 | 57–60 | Software architecture & design patterns |
| Phase 16 | 61–64 | DevOps, Docker, Kubernetes & Cloud |
| Phase 17 | 65–68 | Security engineering |
| Phase 18 | 69–72 | Observability, monitoring & SRE practices |
| Phase 19 | 73–76 | Machine Learning fundamentals |
| Phase 20 | 77–80 | Deep Learning & neural networks |
| Phase 21 | 81–84 | Generative AI & Large Language Models |
| Phase 22 | 85–88 | Data Engineering & pipelines |
| Phase 23 | 89–92 | MLOps & model deployment |
| Phase 24 | 93–96 | Modern languages: Rust, Go & TypeScript |
| Phase 25 | 97–108 | System Design & Career Preparation |

</details>

---

## 🚀 Quick Start

### Option 1: Read Online (Recommended)
The roadmap PDF is automatically compiled and deployed to GitHub Pages on every update.

👉 **[Download / View the PDF Roadmap](https://gkrishna247.github.io/software-engineering-roadmap/roadmap.pdf)**

### Option 2: Clone and Compile Locally
```bash
git clone https://github.com/gkrishna247/software-engineering-roadmap.git
cd software-engineering-roadmap
pdflatex roadmap.tex
```
See the [How to Compile Locally](#-how-to-compile-locally) section for prerequisites.

---

## 📂 Repository Contents

| File | Description |
|------|-------------|
| `roadmap.tex` | The full roadmap source written in LaTeX |
| `roadmap.pdf` | Pre-compiled PDF (auto-generated by GitHub Actions) |
| `prompt-collection.md` | 5 optimized Perplexity AI Deep Research prompts for enhancing the roadmap |
| `.github/workflows/compile-latex.yml` | GitHub Actions workflow that auto-compiles LaTeX to PDF and deploys to GitHub Pages |
| `LICENSE` | MIT License |

---

## 🛠️ How to Compile Locally

### Prerequisites
Install a LaTeX distribution on your system:

- **Linux**: [TeX Live](https://www.tug.org/texlive/)
  ```bash
  sudo apt-get install texlive-full
  ```
- **macOS**: [MacTeX](https://www.tug.org/mactex/)
  ```bash
  brew install --cask mactex
  ```
- **Windows**: [MiKTeX](https://miktex.org/)

### Compile the Roadmap
```bash
# Navigate to the repository directory
cd software-engineering-roadmap

# Compile the LaTeX source to PDF
pdflatex roadmap.tex

# Run twice to resolve cross-references (optional but recommended)
pdflatex roadmap.tex
```

The compiled `roadmap.pdf` will appear in the same directory.

---

## ⚙️ Auto-Compilation (GitHub Actions)

Every time a change is pushed to the repository that modifies `roadmap.tex`, a GitHub Actions workflow (`.github/workflows/compile-latex.yml`) automatically:

1. **Compiles** `roadmap.tex` to `roadmap.pdf` using TeX Live
2. **Commits** the updated PDF back to the repository
3. **Deploys** the latest PDF to **GitHub Pages** for instant online access

This means the [online PDF](https://gkrishna247.github.io/software-engineering-roadmap/roadmap.pdf) is always up to date with the latest version of the roadmap source.

---

## 🤖 Enhancement Prompts

The [`prompt-collection.md`](prompt-collection.md) file contains **5 carefully crafted prompts** designed for use with [Perplexity AI Deep Research](https://www.perplexity.ai/). These prompts help you:

- Validate and update topic coverage against current industry standards
- Generate detailed week-by-week project ideas for specific phases
- Research the best learning resources for each technology stack
- Identify skill gaps and suggest supplementary content
- Benchmark the roadmap against real-world job requirements

**How to use:**
1. Open [Perplexity AI](https://www.perplexity.ai/) and enable **Deep Research** mode
2. Copy a prompt from `prompt-collection.md`
3. Paste it into Perplexity AI and review the research results
4. Use the insights to tailor your study plan or suggest improvements via a [GitHub Issue](https://github.com/gkrishna247/software-engineering-roadmap/issues/new)

---

## 🤝 Contributing

Contributions are welcome! Whether you've spotted an error, want to suggest a new topic, or have a resource recommendation:

1. **Open an Issue** — describe the improvement or correction you'd like to see
2. **Fork & PR** — fork the repository, make your changes to `roadmap.tex`, and open a pull request
3. **Discuss** — share ideas or feedback in [GitHub Discussions](https://github.com/gkrishna247/software-engineering-roadmap/discussions) (if enabled)

Please keep contributions focused, well-reasoned, and aligned with the roadmap's project-based learning philosophy.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

Copyright © 2026 [KRISHNAMOORTHI G](https://github.com/gkrishna247)

---

<div align="center">

⭐ If this roadmap helps you, please consider giving it a star!

</div>
