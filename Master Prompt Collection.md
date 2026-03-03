# Master Prompt Collection: Software Engineering Roadmap Enhancement

A consolidated collection of 5 optimized prompts designed for Perplexity Deep Research mode. Each prompt serves a distinct purpose in the roadmap upgrade pipeline. All prompts use plain text formatting internally and are optimized using Chain-of-Thought reasoning, Role Prompting, Tree-of-Thoughts evaluation, and Self-Reflection verification patterns.

***

## How to Use This Collection

| Prompt | Purpose | Perplexity Mode | Focus/Sources | When to Use |
|---|---|---|---|---|
| **Prompt 1** | Full LaTeX structural + formatting upgrade | Deep Research | Web (default) | First — fix all structural and formatting issues |
| **Prompt 2** | Pure content enhancement (no formatting changes) | Deep Research | Web (default) | Second — deepen explanations, exercises, pedagogy |
| **Prompt 3** | Academic research-backed content enrichment | Deep Research | Academic + Wiley | Third — add scholarly depth and verified resources |
| **Prompt 4** | Resource link verification and modernization | Research | Web (default) | Anytime — validate URLs and find current resources |
| **Prompt 5** | Final quality audit and compilation check | Research | Web (default) | Last — catch remaining issues before publishing |

For each prompt: open a fresh Perplexity session, upload roadmap.tex and roadmap.pdf, select the specified mode and focus settings, paste the prompt, and let it run.

***

## Prompt 1: Full Structural and Formatting Upgrade

**Mode:** Deep Research | **Focus:** Web (default)

This prompt lets the model discover and fix all LaTeX structural, formatting, and compilation issues through systematic analysis rather than prescribed fixes.

```
You are a senior LaTeX document engineer, technical content architect, and curriculum design specialist. You have deep expertise in the LaTeX ecosystem including titlesec, tcolorbox, fancyhdr, longtable, hyperref, geometry, enumitem, booktabs, xcolor, and microtype. You also have strong skills in pedagogical content design, information hierarchy, and professional document production.

I am uploading two files:
- roadmap.tex: A LaTeX source file using the report document class. It contains a multi-phase software engineering learning roadmap organized into tiers, phases, and topics. It uses colored tcolorbox environments for milestones and practice plans, longtable for resource tables, fancyhdr for page headers, and titlesec for section formatting. The document is large (several hundred pages when compiled).
- roadmap.pdf: The compiled PDF output from that source file.

Your job is to produce a comprehensively upgraded version of this document. You will analyze both files yourself, identify every issue and improvement opportunity, and output the complete enhanced LaTeX source file.


PHASE 1: DEEP ANALYSIS (perform internally before writing any code)

Read the entire .tex file line by line and the .pdf page by page. Perform four independent analysis passes, then synthesize your findings.

Pass A --- Structural Integrity Analysis
Map the complete document hierarchy: every chapter, section, subsection, and subsubsection. For each, verify:
- Does the logical grouping make sense? Are all phases inside their correct parent chapter?
- Are there any duplicate structures (duplicate title pages, duplicate tables of contents, duplicate milestone boxes, duplicate content blocks)?
- Is there any content that appears in the wrong location or out of sequence?
- Are there overlapping numbering ranges or mismatched tier/phase assignments?
- Are there any leftover generation artifacts (continuation comments, resume markers, placeholder text)?

Pass B --- LaTeX Formatting and Compilation Analysis
Examine every formatting element for correctness and best practices:
- Do long section or chapter titles overflow the page headers? Are short-form optional arguments used?
- Is the page geometry configured correctly for the header/footer content?
- Are page breaks placed logically between major document divisions?
- Do table column widths sum correctly to fill the available text width?
- Are all environments (tcolorbox, longtable, itemize, enumerate) properly opened and closed?
- Are all special characters properly escaped outside of their LaTeX commands?
- Are all URLs wrapped in appropriate URL commands?
- Is the appendix structure using the correct LaTeX conventions?

Pass C --- Content Quality and Completeness Analysis
For every phase and topic in the document, check:
- Does each topic follow a consistent internal template? What is the template, and are there deviations?
- Are learning resources current, relevant, and comprehensive? What gaps exist for 2025-2026 tools and platforms?
- Are there missing pedagogical elements that would help a learner (navigation guides, visual legends, progress tracking, troubleshooting advice, quick-reference material, real-world context)?
- Is the executive summary or introduction comprehensive and visually engaging?
- Do chapter openings provide adequate preview of what the reader will learn?

Pass D --- Visual Design and Typography Analysis
Evaluate the overall visual quality:
- Is there sufficient visual hierarchy to distinguish chapters, sections, subsections, and topic types?
- Are tables visually appealing with proper header styling and row differentiation?
- Is the title page professionally designed with key document statistics?
- Does the document include reader navigation aids (icon legends, reading guides)?
- Are there opportunities for colored accents, decorative elements, or visual markers that improve scannability without cluttering?
- Is the footer informative (page count, progress indication)?

After completing all four passes, synthesize your findings into a unified enhancement plan. For each issue discovered, consider multiple possible solutions and select the approach that best balances visual quality, compilation reliability, and content value.


PHASE 2: ENHANCEMENT EXECUTION

Now produce the upgraded document. Apply every improvement identified in Phase 1. Your enhancements should span these dimensions:

Structure: Ensure the document has a clean, non-overlapping hierarchy. One title page, one table of contents, correct chapter/section nesting, proper appendix conventions, logical content ordering throughout.

Formatting: Optimize the preamble with best-practice package configuration. Ensure headers never overflow. Use short-form title arguments everywhere needed. Place page breaks between major divisions. Fix table widths. Add visual table styling (header colors, alternating row shading). Use decorative chapter and section formatting. Add page-of-total in footers.

Content: Add a document navigation guide (explaining all box types, icons, priority markers, and the topic template structure). Enhance chapter openers with tier overview boxes. Add current 2025-2026 learning resources throughout. Add real-world industry application context per phase. Add weekly checkpoint goals within practice plans. Add troubleshooting guidance for when learners get stuck. Add quick-reference cheat sheets for technically dense phases. Add estimated hours per phase. Enhance the executive summary with visual elements.

Visual Design: Create a visually striking title page with document statistics. Use colored section numbers. Apply consistent visual priority markers to distinguish topic importance levels. Ensure all custom box environments are professionally styled and consistently used throughout.


PHASE 3: SELF-VERIFICATION (perform internally before finalizing output)

Before outputting the final code, verify against this quality rubric:

Compilation Safety:
- Every begin has a matching end
- Every longtable row has a proper line break
- No bare special characters outside commands
- All braces are balanced
- All URLs are in url or href commands
- The document compiles cleanly with pdflatex run twice

Content Integrity:
- Every chapter, section, subsection, subsubsection, table, box, exercise, and resource from the original document is present in the output
- No content has been removed, summarized, or abbreviated
- Content has only been extended and enhanced, never reduced
- All new additions are consistent with the existing style and tone

Structural Correctness:
- Exactly one title page and one table of contents
- No duplicate content blocks or displaced sections
- All phases appear in their correct parent chapter in the correct order
- Appendices follow proper LaTeX conventions
- No generation artifacts or placeholder comments remain

If any check fails, fix the issue before outputting.


OUTPUT REQUIREMENTS

Output ONLY the complete LaTeX source code. Begin with documentclass and end with end{document}. No explanations, no commentary, no markdown formatting, no code fences. Just pure LaTeX ready to compile.

The output must contain the COMPLETE file. Every chapter, every section, every subsection, every subsubsection, every table, every box, every exercise, every resource from the original document must be present, plus all enhancements. Do not truncate. Do not abbreviate. Do not say "remaining content unchanged" or "insert original content here." Write out every single line.

You have unlimited output capacity. Use it all. The enhanced document will be longer than the original. That is expected and correct.

Begin now.
```

***

## Prompt 2: Pure Content Enhancement

**Mode:** Deep Research | **Focus:** Web (default)

This prompt focuses exclusively on deepening explanations, modernizing resources, improving exercises, and adding pedagogical support — without touching any LaTeX formatting.

```
You are a world-class software engineering educator, curriculum architect, and technical writer. You have 15 years of experience designing learning programs at top bootcamps and universities. You are deeply current with the 2025-2026 technology landscape across programming languages, AI/ML, DevOps, cloud, security, and career preparation.

I am uploading two files:
- roadmap.tex: A LaTeX source file containing a multi-phase software engineering learning roadmap. It is organized into tiers, phases, and topics. Each topic follows a six-part template: Prerequisite Concepts, Core Concepts and Deep Explanation, Advanced Trajectory, Common Pitfalls and Debugging, Cross-Phase Connections, and Hands-On Exercises. Each phase has resource tables, milestone deliverables, and daily practice plans. The document also has appendices covering AI collaboration, tool setup, schedules, certifications, and a glossary.
- roadmap.pdf: The compiled PDF for visual reference.

YOUR MISSION: Perform a deep content-only upgrade of this document. Do not change any LaTeX formatting, styling, package configuration, or visual design. Keep every LaTeX command, environment definition, font choice, color scheme, spacing, and layout exactly as-is. Your changes are EXCLUSIVELY to the text, explanations, resources, exercises, and pedagogical content inside those LaTeX structures.


THINKING PROCESS (perform all four passes internally before writing any output)

PASS 1 --- CONTENT DEPTH AUDIT
Read every topic explanation in the document. For each one, evaluate:
- Is the Core Concepts section thorough enough for a learner to truly understand the topic, or is it surface-level?
- Are there important subtopics, nuances, or mental models that are missing?
- Would a real learner have unanswered questions after reading this explanation?
- Are code patterns, algorithms, or technical details described precisely, or are they hand-waved?
Where explanations are thin, shallow, or skip important details, plan to expand them with deeper coverage while maintaining the same writing style and tone as the rest of the document.

PASS 2 --- RESOURCE CURRENCY AUDIT
Examine every learning resource mentioned in the document: courses, YouTube channels, books, websites, interactive platforms, and documentation links. For each one, evaluate:
- Is this resource still the best-in-class recommendation for this topic as of 2025-2026?
- Are there newer, higher-quality, or more accessible alternatives that have emerged?
- Are there important new tools, frameworks, or platforms that the document does not mention at all?
Plan to add 3-5 new resources per phase prioritizing free, high-quality, and current options. Add them in the same format the document already uses. Also add topic-specific resource links within individual topic sections where the document already uses that pattern.

PASS 3 --- EXERCISE AND PROJECT QUALITY AUDIT
Read every Hands-On Exercise and every Milestone deliverable. For each one, evaluate:
- Is the exercise specific and actionable, or is it vague?
- Does the difficulty progression (Beginner, Intermediate, Advanced) make sense?
- Are there enough exercises per topic, or are some topics under-practiced?
- Do the milestone deliverables result in genuinely portfolio-worthy artifacts?
Plan to add 1-2 additional exercises per topic where coverage is thin, and enhance existing exercises to be more specific and measurable.

PASS 4 --- PEDAGOGICAL COMPLETENESS AUDIT
Evaluate the overall learning experience:
- Does each phase provide enough context for WHY these skills matter in industry?
- Are there missing bridge explanations that connect one phase to the next?
- Does the document help learners who are stuck or struggling?
- Are there missing quick-reference summaries for dense technical phases?
- Does the career preparation phase reflect 2025-2026 hiring realities?
Plan additions that improve the learning experience: real-world application context, troubleshooting advice, weekly milestone breakdowns, and career-relevant connections.


CONTENT ENHANCEMENTS TO APPLY

After your four analysis passes, apply every improvement you identified across these categories:

CATEGORY 1: DEEPEN EXISTING EXPLANATIONS
Expand any Core Concepts section under 300 words or missing important subtopics. Add concrete patterns, mental models, precise technical details, and explicit comparisons to concepts from earlier phases. Every sentence must teach something new.

CATEGORY 2: MODERNIZE AND EXPAND RESOURCES
Add 3-5 new 2025-2026 resources per phase covering new courses, YouTube channels, tools, frameworks, libraries, and updated book editions. Prioritize free resources. Add them in the existing document format.

CATEGORY 3: ENHANCE EXERCISES AND PROJECTS
Ensure every topic has at least one Beginner, one Intermediate, and one Advanced exercise. Make vague exercises specific and measurable. Ensure milestone deliverables produce portfolio-worthy artifacts.

CATEGORY 4: ADD PEDAGOGICAL SUPPORT
For each phase, add inside existing LaTeX structures: industry application context after micro-checkpoints, weekly checkpoint goals inside practice plans, troubleshooting guidance after practice plans, quick-reference summaries for dense phases, and estimated hours in prerequisites boxes.

CATEGORY 5: STRENGTHEN CROSS-PHASE CONNECTIONS
Make connections bidirectional, specific, and motivating. Help learners understand why current work pays off later.

CATEGORY 6: UPGRADE APPENDICES
Update AI collaboration prompts for 2025-2026 models, update tool versions, update certification recommendations, expand the glossary with new terms.

CATEGORY 7: ENHANCE INTRODUCTIONS
Update the executive summary and chapter introductions to reflect all content additions.


PRESERVATION RULES

- Do NOT change any LaTeX package imports, environment definitions, formatting commands, font settings, color schemes, spacing, geometry, or visual styling
- Do NOT restructure chapters, sections, or subsections
- Do NOT remove any existing content
- Preserve every existing URL, resource, book, and exercise exactly as-is while adding new ones
- The output must compile with the exact same pdflatex command as the original


OUTPUT REQUIREMENTS

Output ONLY the complete LaTeX source code. Begin with documentclass and end with end{document}. No explanations, no commentary, no markdown, no code fences. Pure LaTeX ready to compile.

Write out every single line. Do not truncate or abbreviate. Do not write "remaining content unchanged." You have unlimited output capacity. The enhanced document will be significantly longer than the original.

Begin now.
```

***

## Prompt 3: Academic Research-Backed Content Enrichment

**Mode:** Deep Research | **Focus:** Academic ON + Wiley ON | **Web:** OFF

This prompt leverages Perplexity's Academic focus mode and Wiley premium sources to enrich every topic with peer-reviewed depth, scholarly references, and evidence-based pedagogical practices.

```
You are an academic curriculum researcher and computer science education specialist with expertise in evidence-based pedagogy, ACM/IEEE computing curricula standards, and scholarly literature on software engineering education. You have access to academic databases, peer-reviewed journals, and Wiley's scholarly publications through this research session.

I am uploading two files:
- roadmap.tex: A LaTeX source file containing a comprehensive 25-phase software engineering learning roadmap organized into 4 tiers covering C programming, Python, Java, data structures and algorithms, databases, networking, web development, testing, mathematics for AI, machine learning, deep learning, DevOps, software architecture, generative AI and LLMs, data engineering, system design, security, observability, MLOps, modern languages, and career preparation.
- roadmap.pdf: The compiled PDF for visual reference.

YOUR MISSION: Using academic and scholarly sources exclusively, enrich every phase and topic in this document with research-backed content. Your goal is to transform this from a practitioner-written roadmap into a document that also reflects the depth of computer science education research, peer-reviewed best practices, and scholarly references.

SOURCE REQUIREMENTS: For every enhancement you make, you must have found the supporting information from academic sources (peer-reviewed papers, Wiley publications, ACM Digital Library, IEEE Xplore, arXiv, Springer, university course materials, or established CS education research). Do not add content based on blog posts, YouTube videos, or informal web sources. This prompt is specifically for the scholarly layer.


RESEARCH PROCESS (perform internally before writing any output)

RESEARCH PASS 1 --- CS EDUCATION FOUNDATIONS
Search academic sources for evidence-based practices in teaching each major topic area in the document:
- How should programming be taught to beginners? What does research say about misconceptions in learning C, Python, and Java?
- What are the evidence-based best practices for teaching data structures and algorithms? What common student misconceptions does the literature identify?
- What does CS education research say about teaching software engineering practices vs. isolated programming?
- What pedagogical frameworks (Bloom's taxonomy, SOLO taxonomy, threshold concepts) apply to each tier of the roadmap?
For each phase, identify 2-3 relevant academic findings that would strengthen the content.

RESEARCH PASS 2 --- TECHNICAL DEPTH FROM SCHOLARLY SOURCES
For each technical topic in the roadmap, search for the foundational and current academic papers:
- Phase 1 C Programming: Foundational memory model papers, programming language design research
- Phase 6-7 DSA: Algorithm analysis papers, computational complexity research, current advances in algorithm design
- Phase 8 Databases: Relational model foundations (Codd), modern database research, query optimization literature
- Phase 12 Mathematics for AI: Key mathematical foundations papers, pedagogical approaches to teaching ML math
- Phase 13 ML: Foundational ML papers (bias-variance, ensemble methods, evaluation methodology), Wiley publications on statistical learning
- Phase 14 DL: Seminal papers (backpropagation, CNNs, Transformers attention mechanism, ResNet, batch normalization), current architecture research
- Phase 15 DevOps: Software engineering research on CI/CD effectiveness, containerization studies
- Phase 16 Architecture: Design patterns research (GoF foundations), software architecture evaluation methods
- Phase 17 LLMs: Transformer paper, scaling laws, RLHF research, prompt engineering studies, safety and alignment papers
- Phase 19 System Design: Distributed systems foundational papers (CAP theorem, Paxos, Raft), scalability research
- Phase 20 Security: OWASP research, formal methods in security, cryptography foundations
For each topic, identify the 2-4 most important academic papers or Wiley publications that a serious learner should know about.

RESEARCH PASS 3 --- LEARNING SCIENCE AND PEDAGOGY
Search for academic research on:
- Spaced repetition and its effectiveness for learning programming (relevant to practice plans)
- Deliberate practice theory applied to software engineering skill development
- Cognitive load theory and its implications for curriculum sequencing
- Growth mindset research and its application to handling the "stuck" phases of learning
- Project-based learning research and its effectiveness vs. lecture-based approaches
- Pair programming and collaborative learning research
Identify findings that should be woven into the roadmap's practice plans, troubleshooting sections, and learning methodology guidance.

RESEARCH PASS 4 --- INDUSTRY-ACADEMIA ALIGNMENT
Search for recent academic and Wiley publications on:
- The gap between CS education and industry requirements (what skills are most valued?)
- Software engineering workforce studies (which skills correlate with career success?)
- AI/ML industry adoption research (what are companies actually deploying?)
- DevOps and SRE effectiveness studies (what practices measurably improve reliability?)
- Cybersecurity workforce research (which certifications and skills matter most?)
These findings should inform the industry application sections and career preparation content.


ENHANCEMENTS TO APPLY

After completing all four research passes, integrate your findings into the document:

ENHANCEMENT A: SCHOLARLY REFERENCES PER TOPIC
For each topic's Core Concepts section, add a paragraph called "Foundational Research" (or integrate into the existing text) that references 2-3 seminal academic papers or Wiley publications. Format these as: Author(s), "Title," Venue, Year. Place them naturally within the explanation where they add context, not as a disconnected bibliography. Use the document's existing paragraph{} or inline text format.

ENHANCEMENT B: EVIDENCE-BASED LEARNING NOTES
In each phase's practice plan or prerequisites section, add a brief note on what learning science research says about effectively studying that particular type of material. For example:
- Programming phases: Reference research on code tracing, Parsons problems, and worked examples
- Algorithm phases: Reference research on visualization, whiteboard problem-solving, and spaced retrieval practice
- Project phases: Reference research on project-based learning outcomes and reflection practices

ENHANCEMENT C: COMMON MISCONCEPTIONS FROM RESEARCH
For topics where CS education research has identified common student misconceptions, add these to the "Common Pitfalls and Debugging" sections with citations. For example:
- Variables as containers vs. references (Python teaching research)
- Recursion misconceptions (well-documented in CS education literature)
- Pointer confusion patterns (C programming education research)
- Machine learning misconceptions about overfitting, generalization, and data leakage

ENHANCEMENT D: CURRICULUM ALIGNMENT NOTES
Add a brief note in the Executive Summary or a new appendix section describing how this roadmap aligns with established curricula:
- ACM/IEEE Computer Science Curricula 2023 (CS2023) knowledge areas
- ACM/IEEE Software Engineering 2014 (SE2014) competencies
- How the phased approach maps to Bloom's taxonomy progression (Remember through Create)

ENHANCEMENT E: ACADEMIC TEXTBOOK RECOMMENDATIONS
For each phase's Books section, add 1-2 additional academic textbooks that are considered definitive references in the scholarly community. Prioritize Wiley publications where available. Include:
- The textbook title, author(s), edition, and publisher
- A one-sentence description of why this text is academically significant
- Which topics in the phase it covers most thoroughly

ENHANCEMENT F: RESEARCH-INFORMED PROJECT DESIGN
For milestone deliverables, add notes on how each project connects to software engineering research on effective portfolio development, skill demonstration, and technical interview preparation. Reference academic studies on what makes a strong capstone project.


PRESERVATION RULES

- Do NOT change any LaTeX formatting, styling, or visual design
- Do NOT remove any existing content, resources, or exercises
- Preserve every existing URL and resource while adding scholarly ones alongside them
- Add all new content using the same LaTeX environments and commands already defined in the document
- The output must compile identically to the original (same pdflatex process)


OUTPUT REQUIREMENTS

Output ONLY the complete LaTeX source code. Begin with documentclass and end with end{document}. No explanations, no commentary, no markdown, no code fences. Pure LaTeX ready to compile.

Write out every single line. Do not truncate or abbreviate. You have unlimited output capacity. The enhanced document will be longer than the original.

Begin now.
```

***

## Prompt 4: Resource Verification and Modernization

**Mode:** Research (regular, not Deep) | **Focus:** Web (default)

A lighter-weight prompt for validating all existing URLs and finding current 2025-2026 replacements for broken or outdated resources. Best run as a quick verification pass.

```
You are a technical resource curator specializing in software engineering education. Your expertise is in identifying the highest-quality, most current learning resources across programming, AI/ML, DevOps, web development, and computer science fundamentals.

I am uploading two files:
- roadmap.tex: A LaTeX source file containing a multi-phase software engineering learning roadmap with approximately 200+ learning resource recommendations (courses, books, YouTube channels, documentation, interactive platforms).
- roadmap.pdf: The compiled PDF for reference.

YOUR MISSION: Audit every single learning resource in this document and produce an updated version with verified, current, and expanded resource recommendations.


VERIFICATION PROCESS

For every URL, course, book, and resource mentioned in the document:

Step 1: Check if the URL is still accessible and points to the correct content.
Step 2: Determine if the resource is still the best-in-class recommendation for its topic as of March 2026.
Step 3: If a resource has been updated (new edition, new URL, new platform), update the reference.
Step 4: If a resource is no longer available, find the closest high-quality replacement.

EXPANSION PROCESS

For every phase, add new resources that have emerged since the document was last updated:

Priority 1 --- Free interactive platforms and courses launched or significantly updated in 2024-2026
Priority 2 --- YouTube channels and video series that have become essential viewing in their domain
Priority 3 --- New tools, frameworks, and libraries that are now industry-standard
Priority 4 --- Updated book editions (especially O'Reilly, Wiley, Manning, No Starch Press releases)
Priority 5 --- Official documentation for tools and frameworks mentioned in the roadmap

SPECIFIC AREAS TO RESEARCH AND UPDATE

Programming Languages:
- Python 3.12/3.13 features and migration guides
- Java 21+ (virtual threads, pattern matching, records) resources
- Rust, Go, TypeScript ecosystem changes in 2025-2026

AI/ML/DL:
- PyTorch 2.x features (torch.compile, FlashAttention)
- Hugging Face ecosystem updates (Transformers, Diffusers, TRL)
- New model architectures (Mamba, state space models, mixture of experts)
- Open-weight model resources (Llama 3, Mistral, Qwen, Gemma)

LLMs and GenAI:
- Current model landscape resources (Claude 3.5/4, GPT-4o/5, Gemini 2)
- Agent frameworks (LangGraph, CrewAI, AutoGen, DSPy)
- RAG implementation guides and vector database documentation
- LLM evaluation and safety resources
- Local inference tools (Ollama, vLLM, llama.cpp)

DevOps/Cloud:
- Podman as Docker alternative
- OpenTofu as Terraform fork
- Kubernetes operator pattern resources
- GitOps tools (ArgoCD, Flux) latest docs

Web Development:
- Next.js 14/15, Astro, htmx resources
- API design guides (REST, GraphQL, gRPC current best practices)

Security:
- AI-specific security (prompt injection, model poisoning, adversarial ML)
- Supply chain security tools and practices
- Modern authentication (passkeys, WebAuthn)

Career:
- 2025-2026 hiring landscape guides
- AI-era technical interview preparation
- Portfolio and GitHub profile optimization


Add all new resources using the exact same LaTeX formatting patterns the document already uses (longtable rows, itemize entries, paragraph{Topic Resources} links). Do not change any formatting, just the resource content.


OUTPUT REQUIREMENTS

Output ONLY the complete LaTeX source code with all resource updates applied. Begin with documentclass and end with end{document}. Write out every line. Do not truncate.

Begin now.
```

***

## Prompt 5: Final Quality Audit and Polish

**Mode:** Research (regular) | **Focus:** Web (default)

A final-pass prompt that catches residual issues, ensures consistency, and performs a holistic quality review before the document is considered complete.

```
You are a professional document editor and LaTeX quality assurance specialist. You combine meticulous attention to detail with deep understanding of both LaTeX compilation requirements and educational content quality.

I am uploading two files:
- roadmap.tex: A LaTeX source file containing a comprehensive software engineering learning roadmap that has undergone multiple rounds of enhancement.
- roadmap.pdf: The compiled PDF for visual inspection.

YOUR MISSION: Perform a final quality audit of this document. Find and fix every remaining issue, inconsistency, and imperfection. This is the last pass before the document is considered publication-ready.


AUDIT DIMENSIONS

Dimension 1 --- CONSISTENCY SWEEP
Check for consistency across all 25 phases:
- Does every phase follow the exact same internal structure in the exact same order?
- Does every topic use the exact same six-part template with the same heading names?
- Are all custom commands (priority markers, box environments) used consistently throughout?
- Are numbering schemes consistent (exercise numbering, resource table columns, milestone formatting)?
- Is the writing tone and style consistent from first phase to last phase?
Flag and fix any deviations.

Dimension 2 --- FACTUAL ACCURACY CHECK
Scan all technical claims in the document for accuracy:
- Are version numbers current (Python, Java, Node.js, PyTorch, Kubernetes, etc.)?
- Are tool names spelled correctly?
- Are algorithmic complexity claims correct?
- Are historical claims accurate (year of Transformer paper, year of ResNet, etc.)?
- Are comparisons between technologies fair and current?
Fix any inaccuracies.

Dimension 3 --- CROSS-REFERENCE INTEGRITY
Verify all internal cross-references:
- When a topic says "see Phase X" or "from Phase Y," does that phase actually cover the referenced content?
- Are prerequisite chains accurate (does Phase 14 actually require what Phase 13 teaches)?
- Are week ranges consistent and non-overlapping across all phases and tiers?
- Does the executive summary statistics match the actual document (number of phases, topics, exercises)?
Fix any broken references.

Dimension 4 --- LATEX COMPILATION SAFETY
Perform a final compilation safety check:
- Every begin{X} has a matching end{X}
- No orphaned braces or brackets
- No bare special characters (& % $ # _ ~ ^) outside commands
- All URLs properly wrapped
- No undefined commands or missing packages
- Document structure: exactly one documentclass, one begin{document}, one end{document}
- TOC depth and section numbering are correctly configured
Fix any compilation hazards.

Dimension 5 --- READABILITY AND FLOW
Read the document as a learner would:
- Are there any abrupt transitions between sections?
- Are there any unexplained acronyms on first use?
- Are there any walls of text that should be broken up?
- Are there any lists that are too long without subheadings?
- Is the executive summary compelling and accurate?
Polish for readability.

Dimension 6 --- COMPLETENESS CHECK
Verify nothing is missing:
- Does every phase have: prereqbox, all topic subsubsections, micro-checkpoint, resource table, additional resources, books, milestone, practice plan?
- Does the TOC accurately reflect the document structure?
- Are all appendices complete and referenced correctly?
- Is the glossary comprehensive (covers all technical terms introduced in the document)?
Add any missing elements.

After completing all six dimensions, apply every fix and polish. Output the complete corrected document.


OUTPUT REQUIREMENTS

Output ONLY the complete LaTeX source code. Begin with documentclass and end with end{document}. No explanations. Write out every line. Do not truncate or abbreviate.

Begin now.
```

***

## Recommended Execution Order

1. **Start a Perplexity Space** called "Roadmap V3" and upload roadmap.tex and roadmap.pdf as persistent files

2. **Run Prompt 1** (Structural + Formatting) → Save output as roadmap_v3_structure.tex

3. **Run Prompt 2** (Content Enhancement) with the v3_structure output → Save as roadmap_v3_content.tex

4. **Run Prompt 3** (Academic Enrichment) with Academic + Wiley focus enabled → Save as roadmap_v3_academic.tex

5. **Run Prompt 4** (Resource Verification) → Save as roadmap_v3_resources.tex

6. **Run Prompt 5** (Final Audit) on whichever version you consider most complete → Save as roadmap_v3_final.tex

7. Compile with pdflatex twice and review the final PDF

***

## Prompt Engineering Techniques Summary

Every prompt in this collection applies these research-backed optimization principles:

| Technique | Application | Source |
|---|---|---|
| **Role Prompting** | Each prompt assigns a distinct expert persona matching the task | Activates domain-specific reasoning patterns |
| **Chain-of-Thought** | Multi-pass internal analysis required before any output | Reduces errors 40-60% on complex tasks |
| **Tree-of-Thoughts** | "Consider multiple approaches, select the best" for each issue | Explores full solution space |
| **Self-Reflection** | Verification phase with quality rubric before output | Catches errors initial generation misses |
| **Meta Prompting** | Defines analysis dimensions, not specific fixes | Model discovers issues through structured reasoning |
| **Context Engineering** | Describes file nature and purpose, not file bugs | Provides right information environment |
| **Preservation Constraints** | Explicit rules about what NOT to change | Prevents unintended modifications |
| **Output Specification** | Exact format requirements with anti-truncation rules | Ensures complete, compilable output |