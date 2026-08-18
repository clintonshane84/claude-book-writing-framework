# Claude Book Writing Framework

A complete, production-ready framework for collaboratively writing books with Claude AI. This repository serves as a **template** for new book writing projects—when you start a new book, you'll clone this repository and adapt it for your specific project.

## Overview

This framework provides everything needed to write, review, and publish a book using Claude Code:

- **Pre-writing validation** to ensure readiness
- **Four-phase writing process** (Plan → Write → Review → Publish)
- **Comprehensive writing guidance** balancing technical, craft, and process elements
- **9 specialized skills** for different writing and editing tasks
- **Structured organization** for chapters, drafts, and resources
- **Complete documentation** at every step

## Quick Start

### For Template Users (Starting a New Book)

1. **Clone this repository** for your new book project
2. **Read CLAUDE.md** to understand the framework
3. **Provide your inputs**:
   - Book concept and target audience
   - 1-2 writing samples (to establish voice)
   - Partial/full chapter drafts (if available)
   - Any research or reference materials
4. **Organize global resources** in `/inputs/`:
   - Draft pages in `/inputs/draft-pages/`
   - Research materials in `/inputs/research/`
   - Reference materials in `/inputs/references/`
   - These are automatically available to Claude when writing
5. **Work through validation** (see `/framework/validation-checklist.md`)
6. **Execute the four-phase process**:
   - Phase 1: Plan (outline, structure, targets)
   - Phase 2: Write (chapter-by-chapter drafting with global context)
   - Phase 3: Review (edit, polish, consistency)
   - Phase 4: Publish (compile, format, distribute)

### For Framework Developers (Contributing)

1. Explore the framework structure and documentation
2. Review the four-phase process (each in its own file)
3. Examine the 9 specialized skills
4. Suggest improvements or extensions

## Repository Structure

```
claude-framework-book-writing/
│
├── README.md                                    # This file
├── CLAUDE.md                                    # Entry point (read first!)
│
├── framework/                                   # Core framework documentation
│   ├── writing-rules.md                         # Writing standards and best practices
│   ├── persona-writing-style.md                 # Template for author voice documentation
│   ├── writing-tools.md                         # Markdown format and technical reference
│   ├── directory-structure.md                   # How to organize book content
│   ├── resources-guide.md                       # Managing images, data, and materials
│   ├── validation-checklist.md                  # Pre-writing validation requirements
│   │
│   ├── process-plan.md                          # Phase 1: Planning
│   ├── process-write.md                         # Phase 2: Writing
│   ├── process-review.md                        # Phase 3: Review and Editing
│   ├── process-publish.md                       # Phase 4: Publishing
│   │
│   └── skills/                                  # Specialized skills for different tasks
│       ├── skill-book-planning.md               # Organize structure, create outlines
│       ├── skill-book-writing.md                # Draft chapters, develop content
│       ├── skill-book-reviewing.md              # Edit for quality and consistency
│       ├── skill-book-research.md               # Find and integrate research
│       ├── skill-content-editing.md             # Refine prose and language
│       ├── skill-chapter-organization.md        # Improve structure and flow
│       ├── skill-fact-checking.md               # Verify accuracy and sources
│       ├── skill-copyediting.md                 # Polish grammar and formatting
│       └── skill-bibliography.md                # Manage citations and bibliography
│
└── inputs/                                      # Global resources for entire book (per-project)
    ├── README.md                                # Guide for organizing global resources
    ├── draft-pages/                             # Partially written chapters or pages
    ├── research/                                # Research materials, reports, findings
    └── references/                              # Reference materials, examples, inspiration
```

## Key Documents

### Start Here
- **CLAUDE.md** - Main entry point with validation checklist and process overview
- **validation-checklist.md** - What to verify before starting writing

### Global Resources
- **inputs/README.md** - Guide for organizing draft pages, research, and references
  - Automatically available to Claude when writing chapters
  - Supports research-driven writing and completion of partial drafts

### Core Guidance
- **writing-rules.md** - Technical, craft, and process guidance
- **persona-writing-style.md** - Template for documenting your writing voice
- **writing-tools.md** - Markdown format and technical standards
- **directory-structure.md** - How to organize chapters and resources
- **resources-guide.md** - Managing images, data, and reference materials

### Four-Phase Process
- **process-plan.md** - Phase 1: Planning book structure and outline
- **process-write.md** - Phase 2: Writing chapters
- **process-review.md** - Phase 3: Editing and polishing
- **process-publish.md** - Phase 4: Publishing and distribution

### Specialized Skills (Use as Needed)
- **skill-book-planning.md** - Structure your book
- **skill-book-writing.md** - Draft chapters
- **skill-book-reviewing.md** - Comprehensive chapter review
- **skill-book-research.md** - Gather research materials
- **skill-content-editing.md** - Refine prose
- **skill-chapter-organization.md** - Improve flow
- **skill-fact-checking.md** - Verify accuracy
- **skill-copyediting.md** - Polish grammar
- **skill-bibliography.md** - Manage citations

## The Four-Phase Process

### Phase 1: Plan
Map the book's structure, create detailed chapter outline, and establish writing targets.
- **Read**: `/framework/process-plan.md`
- **Use Skill**: `skill-book-planning.md`
- **Output**: Outline, writing timeline, chapter targets

### Phase 2: Write
Draft chapters one-by-one, following your outline and established voice. Claude automatically uses all files in `/inputs/` for research, examples, and context.
- **Read**: `/framework/process-write.md`
- **Use Skill**: `skill-book-writing.md`
- **Global Context**: All materials in `/inputs/` automatically inform writing
- **Output**: Complete chapter drafts informed by your research and references

### Phase 3: Review
Edit chapters for clarity, consistency, and quality at multiple levels.
- **Read**: `/framework/process-review.md`
- **Use Skills**: 
  - `skill-book-reviewing.md` - Overall review
  - `skill-content-editing.md` - Language refinement
  - `skill-chapter-organization.md` - Structure improvement
  - `skill-copyediting.md` - Grammar and polish
  - `skill-fact-checking.md` - Accuracy verification
- **Output**: Polished, publication-ready chapters

### Phase 4: Publish
Compile your chapters into a complete manuscript and prepare for distribution.
- **Read**: `/framework/process-publish.md`
- **Output**: PDF, EPUB, HTML, or print-ready manuscript

## Global Resources for Your Book

The framework includes a dedicated `/inputs/` folder where you can organize materials used throughout your entire book:

### What Goes in `/inputs/`

**Draft Pages** (`/inputs/draft-pages/`)
- Partially written chapters or sections
- Existing openings or key passages you want to preserve
- Previous attempts or rough outlines
- Sections you want Claude to expand or refine

**Research Materials** (`/inputs/research/`)
- Academic papers and studies
- Interview transcripts and expert quotes
- Statistical data and findings
- Case studies and real-world examples
- Industry reports and research notes

**Reference Materials** (`/inputs/references/`)
- Writing style examples you want to match
- Chapter structure examples or templates
- Technical terminology definitions
- Inspirational passages or quotes
- Similar books or outlines for reference

### How Claude Uses Global Resources

When you use **skill-book-writing.md** to draft chapters:
1. Claude automatically reads ALL files in `/inputs/`
2. These materials inform chapter writing without manual reference
3. Draft pages guide chapter completion
4. Research findings are naturally integrated
5. Reference materials ensure consistent voice and style

**Important**: You don't need to mention `/inputs/` files in your requests—Claude automatically considers them.

### Example Usage

**Scenario 1: Research-Driven Chapter**
- You place study findings in `/inputs/research/study-findings.md`
- You place statistics in `/inputs/research/statistics-2024.md`
- Claude writes Chapter 3 and naturally integrates the research
- Claims are supported by your provided data

**Scenario 2: Completing Partial Drafts**
- You have a partial chapter opening in `/inputs/draft-pages/chapter-04-opening.md`
- You request Chapter 4 to be written
- Claude reads your partial draft and completes it in your voice
- Your existing opening is preserved and expanded upon

**Scenario 3: Maintaining Writing Style**
- You place your writing examples in `/inputs/references/writing-examples.md`
- You place chapter structure guides in `/inputs/references/structure-examples.md`
- Claude writes chapters matching your established style and structure
- Consistency is maintained across all chapters

## Writing Rules and Standards

The framework emphasizes:

### Clarity and Readability
- Clear, accessible sentences focused on reader comprehension
- Master each sentence and paragraph individually
- "Show, don't tell"—use examples and details

### Technical Standards
- GitHub-flavored Markdown (.md files)
- Consistent formatting and structure
- Proper organization of chapters, drafts, and resources

### Craft and Style
- Authentic writing voice (documented in persona-writing-style.md)
- Consistent tone and vocabulary
- Varied sentence length for rhythm and pacing

### Process and Workflow
- Multiple revision passes (content, clarity, voice, polish)
- Regular git commits
- Clear separation of drafts from published chapters

See `/framework/writing-rules.md` for comprehensive guidance.

## Book Organization

When you start a new book project, organize it like this:

```
your-book-project/
│
├── CLAUDE.md                     # Entry point (same as template)
├── README.md                     # Your book project description
├── framework/                    # Framework files (reference only)
│   └── [All framework files - used as reference]
│
├── inputs/                       # Global resources for entire book
│   ├── README.md                # Guide for organizing global resources
│   ├── draft-pages/             # Partially written chapters or pages
│   ├── research/                # Research materials, reports, findings
│   └── references/              # Reference materials, examples, inspiration
│
├── book/                         # Your actual book content
│   ├── 01-introduction/
│   │   ├── chapter.md           # Main chapter content
│   │   ├── drafts/              # Work-in-progress versions
│   │   └── resources/           # Images and data for this chapter
│   │
│   ├── 02-chapter-one/
│   │   ├── chapter.md
│   │   ├── drafts/
│   │   └── resources/
│   │
│   └── [continuing chapters...]
│
└── resources/                    # Optional: shared resources
    ├── research/                # Research materials by topic
    ├── images/                  # Shared images
    └── personas/                # Your persona-writing-style.md
```

### Global Resources in `/inputs/`
The `/inputs/` folder contains materials that inform the entire book:
- **Draft pages**: Partially written chapters or sections
- **Research**: Academic papers, studies, interview notes, statistics
- **References**: Writing examples, style guides, inspirational passages

When using skill-book-writing.md to draft chapters, Claude **automatically reads all files in `/inputs/`** and uses them as context. This enables research-driven writing and supports completion of partially-written content without manual reference.

### Chapter Organization
Each chapter gets its own numbered folder:
- `chapter.md` - Final, published chapter content
- `drafts/` - Work-in-progress and revision versions
- `resources/` - Images, data, and supporting materials for the chapter

See `/framework/directory-structure.md` for detailed organization guidance.

## Getting Started: Step-by-Step

### Step 1: Validate Your Inputs
Before writing, verify you have:
- [ ] Book topic/concept clearly defined
- [ ] 1-2 writing samples showing your voice
- [ ] Target audience identified
- [ ] Partial or full chapter drafts (if available)
- [ ] Research materials or resources needed
- [ ] Approximate chapter count
- [ ] Global resources organized in `/inputs/` (if applicable):
  - [ ] Draft pages in `/inputs/draft-pages/`
  - [ ] Research materials in `/inputs/research/`
  - [ ] References in `/inputs/references/`

See `/framework/validation-checklist.md` for full checklist and `/inputs/README.md` for organizing global resources.

### Step 2: Document Your Voice
Create or update `persona-writing-style.md` with:
- Your writing voice and tone
- Target audience
- Book genre and purpose
- Core themes
- Writing examples
- Consistency guidelines

See `/framework/persona-writing-style.md` for the template.

### Step 3: Plan Your Book
Follow Phase 1 to:
- Define book structure (chapters, topics, flow)
- Create detailed chapter outline
- Set writing targets and timeline
- Prepare for writing

See `/framework/process-plan.md` for detailed planning steps.

### Step 4: Write Your Chapters
Follow Phase 2 to:
- Draft chapters one-by-one
- Self-review each chapter
- Commit drafts to git
- Maintain consistency with persona

See `/framework/process-write.md` for writing workflow.

### Step 5: Review and Polish
Follow Phase 3 to:
- Review chapters at multiple levels (content, clarity, voice, grammar)
- Make revisions
- Check consistency across all chapters
- Prepare for publication

See `/framework/process-review.md` for review process.

### Step 6: Publish
Follow Phase 4 to:
- Compile chapters into complete manuscript
- Export to desired formats (PDF, EPUB, HTML)
- Prepare publication materials
- Publish and distribute

See `/framework/process-publish.md` for publishing steps.

## Using Specialized Skills

The framework includes 9 specialized skills for different tasks:

| Skill | Use When | Output |
|-------|----------|--------|
| **skill-book-planning.md** | Planning book structure | Outline, timeline, targets |
| **skill-book-writing.md** | Drafting chapters | Full chapter content |
| **skill-book-reviewing.md** | Comprehensive chapter review | Detailed feedback and suggestions |
| **skill-book-research.md** | Gathering research materials | Organized sources by chapter |
| **skill-content-editing.md** | Improving prose and language | Refined, polished text |
| **skill-chapter-organization.md** | Improving structure and flow | Better organized chapter |
| **skill-fact-checking.md** | Verifying accuracy | Verified claims and citations |
| **skill-copyediting.md** | Polish grammar and formatting | Corrected, publication-ready text |
| **skill-bibliography.md** | Managing citations | Complete bibliography |

Each skill includes:
- When to use it
- What it does
- How to use it
- Common outputs and examples
- Related skills

## Writing Rules Summary

### Technical
- Use GitHub-flavored Markdown
- One chapter per folder (01-, 02-, 03-...)
- Main content in `chapter.md`
- Drafts in `drafts/` subfolder
- Resources in `resources/` subfolder

### Craft
- Write clear, accessible sentences
- Use active voice (prefer over passive)
- Show, don't tell
- Vary sentence and paragraph length
- One main idea per paragraph

### Voice
- Write in your authentic voice
- Document voice in persona-writing-style.md
- Maintain consistency across chapters
- Be conversational or formal as appropriate
- Let personality shine through

### Process
- Draft quickly, revise thoroughly
- Multiple revision passes (content → clarity → polish)
- Read aloud to catch awkward phrasing
- Commit work frequently to git
- Leave room for discovery while writing

See `/framework/writing-rules.md` for comprehensive guidance.

## How Claude Works with This Framework

When Claude encounters this framework in a repository:

1. **Reads CLAUDE.md** to understand the book writing process
2. **Validates inputs** - Checks that necessary files and information are provided
3. **Asks clarifying questions** if anything is unclear
4. **Executes the four-phase process** systematically
5. **Uses specialized skills** as needed during each phase
6. **Maintains consistency** with established voice and style
7. **Commits work** regularly with clear messages

The framework ensures Claude understands:
- What makes effective book writing
- How to capture and maintain an author's voice
- How to structure and organize content
- How to handle the complete writing lifecycle

## Customizing the Framework

This is a template. For your specific book project, you might:

- Add additional writing rules specific to your genre
- Create custom checklists for your type of book
- Add more specialized skills for unique needs
- Adjust the four-phase process if needed
- Include genre-specific writing conventions

**Important**: Keep the core structure and phases. The validation, planning, writing, review, and publishing phases work for all book types.

## Framework Files Reference

### Core Guidance Files
| File | Lines | Purpose |
|------|-------|---------|
| CLAUDE.md | 150+ | Entry point and orchestration |
| writing-rules.md | 400+ | Complete writing guidance |
| persona-writing-style.md | 350+ | Voice documentation template |
| writing-tools.md | 350+ | Technical reference |
| directory-structure.md | 300+ | Organization guide |
| resources-guide.md | 350+ | Resource management |
| validation-checklist.md | 350+ | Pre-writing validation |

### Process Files
| File | Lines | Phase |
|------|-------|-------|
| process-plan.md | 400+ | Phase 1 - Planning |
| process-write.md | 450+ | Phase 2 - Writing |
| process-review.md | 550+ | Phase 3 - Review |
| process-publish.md | 400+ | Phase 4 - Publishing |

### Skills Files
All 9 skills: 200-300 lines each with practical guidance

**Total Framework**: 6,500+ lines of comprehensive documentation

## Best Practices

### Before Starting
- [ ] Read CLAUDE.md completely
- [ ] Understand the four-phase process
- [ ] Complete validation checklist
- [ ] Document your writing voice
- [ ] Gather research materials

### During Writing
- [ ] Follow the outline loosely (not rigidly)
- [ ] Ensure `/inputs/` is organized with research and references
- [ ] Write regularly and commit frequently
- [ ] Read previous chapters for continuity
- [ ] Refer to persona-writing-style.md often
- [ ] Don't perfect while drafting
- [ ] Claude automatically uses `/inputs/` materials for context

### During Review
- [ ] Read complete chapters without stopping first
- [ ] Review at multiple levels (content, clarity, voice, grammar)
- [ ] Check consistency across chapters
- [ ] Fix one type of issue at a time
- [ ] Don't over-edit

### Before Publishing
- [ ] Read complete book start to finish
- [ ] Verify all images and resources
- [ ] Check all citations and bibliography
- [ ] Test file formats (PDF, EPUB, etc.)
- [ ] Do final proofread

## Common Questions

### Q: Is this for all book genres?
**A**: Yes. The framework is genre-agnostic and works for fiction, non-fiction, self-help, educational, memoir, technical, and more.

### Q: Can I use this solo (without Claude)?
**A**: Yes, it's comprehensive writing guidance that Claude uses, but you can follow it independently.

### Q: How long does a book take?
**A**: Depends on length and complexity. Plan 4-12 weeks for a typical book (10-15 chapters).

### Q: Can I modify the framework?
**A**: Yes, adapt it for your needs. Keep core phases but customize guidance.

### Q: What if I get stuck?
**A**: Use the specialized skills. Each provides detailed help for specific challenges.

### Q: How do I use global resources?
**A**: Place your draft pages, research, and reference materials in the `/inputs/` folder (organized in subfolders). Claude automatically reads all files in `/inputs/` when writing chapters. No need to manually reference them—they inform the writing automatically.

### Q: What should go in `/inputs/`?
**A**: Anything that informs your book: partial chapter drafts, research findings, interview notes, statistics, writing style examples, and reference materials. See `/inputs/README.md` for detailed guidance.

## Support and Feedback

This is a living framework. If you:
- Find something unclear
- Have suggestions for improvement
- Discover missing guidance
- Want additional skills

Please open an issue or contribute improvements to the template.

## Success Criteria

Your book project is successful when:
- ✅ All chapters are drafted in your authentic voice
- ✅ Content is reviewed and refined for clarity
- ✅ Writing follows the established rules and guidelines
- ✅ Final manuscript is ready for publication
- ✅ You're satisfied with the quality and voice

## Start Writing

1. **Clone this repository** for your book project
2. **Read CLAUDE.md** - It's your roadmap
3. **Complete validation** - Make sure you're ready
4. **Execute Phase 1** - Plan your book
5. **Begin Phase 2** - Start writing

Good luck with your book project! This framework is designed to help you write clearly, authentically, and consistently, with Claude as your collaborative partner.

---

**Learn More**: See CLAUDE.md for detailed instructions on every phase of the process.
