# Claude Book Writing Framework

## Overview

This is a template repository for writing books collaboratively with Claude AI. Each new book project creates a repository cloned from this template, allowing an agent to understand the book writing framework, rules, processes, and available tools.

When you clone this template for a new book project, Claude will:
1. Read this CLAUDE.md file to understand the framework
2. Reference supporting framework files for detailed guidance
3. Help you plan, write, review, and publish your book

---

## Essential Rules

### Writing Standards
1. **Clarity and Readability**: Write clear, easy-to-read sentences and paragraphs focused on reader comprehension
2. **Mastery Through Iteration**: Perfect each sentence and paragraph individually before moving forward
3. **Format**: All book content written in GitHub-flavored Markdown (.md files)
4. **Consistent Style**: Follow the persona and writing style defined in your book's `persona-writing-style.md`

### Framework Organization
- Framework files live in `/framework/` (guides, rules, processes, skills)
- Book content lives in `/book/` (chapters, drafts, resources)
- Each chapter has its own numbered folder: `01-intro/`, `02-chapter-one/`, etc.

---

## Getting Started: Validation Checklist

**Before Claude begins writing, these items MUST be verified:**

### Required Input Files
- [ ] **Book page drafts**: At least one complete or partial page/chapter draft showing the book's direction
- [ ] **Writing examples**: 1-2 page samples written by you in your natural voice and style
- [ ] **Persona documentation**: Completed `persona-writing-style.md` with your writing style, tone, target audience, and book themes
- [ ] **Resources**: Any documents, research, data, images, or reference materials the book needs

### Validation Steps
1. **Check Drafts**: Confirm book drafts exist and are clear about intended content and scope
2. **Analyze Persona**: Review writing examples to extract and document your unique voice, audience, and style
3. **Verify Resources**: Ensure all necessary reference materials are available
4. **Ask Questions**: If anything is unclear or missing, ask the user to clarify or provide additional context
5. **Confirm Before Starting**: Once all inputs are validated, explicitly confirm with the user before moving to the Plan phase

---

## Book Writing Process

The book is written through four interconnected phases, each with detailed steps:

### Phase 1: Plan
Map the book's structure, outline chapters, and establish writing targets.
→ See `/framework/process-plan.md` for detailed planning steps

### Phase 2: Write
Draft chapters one by one, following the writing rules and persona.
→ See `/framework/process-write.md` for detailed writing steps

### Phase 3: Review
Edit chapters for clarity, consistency, and quality.
→ See `/framework/process-review.md` for detailed review steps

### Phase 4: Publish
Compile the final book, format for publication, and prepare for release.
→ See `/framework/process-publish.md` for detailed publishing steps

Each phase contains sub-steps and uses specific skills to accomplish its goals.

---

## Framework Files Reference

### Core Guidance Files
| File | Purpose |
|------|---------|
| `/framework/writing-rules.md` | Writing rules, best practices, and style guidance |
| `/framework/persona-writing-style.md` | Template for documenting author voice, tone, and style |
| `/framework/writing-tools.md` | Supported formats, tools, and markdown conventions |
| `/framework/directory-structure.md` | How to organize book projects and chapter folders |
| `/framework/resources-guide.md` | Managing images, assets, and reference materials |
| `/framework/validation-checklist.md` | Detailed validation checklist (expanded version) |

### Process Files
| File | Purpose |
|------|---------|
| `/framework/process-plan.md` | Step-by-step planning process |
| `/framework/process-write.md` | Step-by-step writing process |
| `/framework/process-review.md` | Step-by-step review process |
| `/framework/process-publish.md` | Step-by-step publishing process |

### Skills Files
Claude has specialized skills available to help with book writing tasks:

| Skill | Purpose |
|-------|---------|
| `/framework/skills/skill-book-planning.md` | Organize book structure, create outlines, set writing goals |
| `/framework/skills/skill-book-writing.md` | Draft chapters with focus on style, clarity, and flow |
| `/framework/skills/skill-book-reviewing.md` | Edit chapters for consistency, clarity, and quality |
| `/framework/skills/skill-book-research.md` | Research topics, find sources, organize research materials |
| `/framework/skills/skill-content-editing.md` | Refine prose, improve sentences, strengthen narrative |
| `/framework/skills/skill-chapter-organization.md` | Structure chapters, organize sections, improve flow |
| `/framework/skills/skill-fact-checking.md` | Verify claims, check accuracy, validate information |
| `/framework/skills/skill-copyediting.md` | Polish text, fix grammar, ensure style consistency |
| `/framework/skills/skill-bibliography.md` | Manage citations, create bibliographies, track sources |

---

## Quick Navigation

**For new books**: Start with validation checklist above, then see `/framework/validation-checklist.md` for details

**For writing rules**: See `/framework/writing-rules.md`

**For persona/style**: See `/framework/persona-writing-style.md`

**For processes**: See `/framework/process-*.md` files for each phase

**For skills**: See `/framework/skills/` folder for detailed skill documentation

**For book structure**: See `/framework/directory-structure.md`

**For resources**: See `/framework/resources-guide.md`

---

## Starting a New Book Project

1. **Clone** this template repository for your new book
2. **Add book inputs**: Provide drafts, writing examples, persona docs, and resources
3. **Run validation**: Claude verifies all required inputs are present
4. **Confirm start**: Once validated, begin the Plan phase
5. **Execute process**: Follow Plan → Write → Review → Publish phases
6. **Iterate**: Each phase may loop back for refinement

---

## Success Criteria

Your book project is successful when:
- ✅ All chapters are drafted according to your persona and style
- ✅ Content is reviewed and refined for clarity and consistency
- ✅ Writing follows the established rules and guidelines
- ✅ Final manuscript is ready for publication
- ✅ You're satisfied with the quality and voice throughout

---

**Next Step**: If this is a new book project, provide your drafts, writing examples, and persona information so Claude can begin validation and planning.
