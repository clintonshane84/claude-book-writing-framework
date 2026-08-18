# Directory Structure and Organization

This document explains how to organize your book project repository for efficient writing, reviewing, and publishing.

---

## Overall Repository Structure

```
your-book-project/
│
├── README.md                          # Project overview and quick start
├── CLAUDE.md                          # Main framework file (read first)
│
├── framework/                         # Framework files (reference only)
│   ├── writing-rules.md              # Writing rules and best practices
│   ├── persona-writing-style.md      # Your writing voice guide
│   ├── writing-tools.md              # Markdown and technical tools
│   ├── directory-structure.md        # This file
│   ├── resources-guide.md            # How to manage resources/images
│   ├── validation-checklist.md       # Pre-writing validation
│   ├── process-plan.md               # Planning phase
│   ├── process-write.md              # Writing phase
│   ├── process-review.md             # Review phase
│   ├── process-publish.md            # Publishing phase
│   └── skills/                       # Claude Skills
│       ├── skill-book-planning.md
│       ├── skill-book-writing.md
│       ├── skill-book-reviewing.md
│       ├── skill-book-research.md
│       ├── skill-content-editing.md
│       ├── skill-chapter-organization.md
│       ├── skill-fact-checking.md
│       ├── skill-copyediting.md
│       └── skill-bibliography.md
│
├── book/                              # Your actual book content
│   ├── 01-intro/                     # Chapter 1
│   │   ├── chapter.md                # Main chapter content
│   │   ├── drafts/                   # Work-in-progress versions
│   │   │   ├── draft-v1-opening.md
│   │   │   ├── draft-v2-revised.md
│   │   │   └── draft-v3-final.md
│   │   └── resources/                # Images, data, and references
│   │       ├── image-hero.png
│   │       ├── diagram-overview.svg
│   │       └── sources.md
│   │
│   ├── 02-chapter-one/               # Chapter 2
│   │   ├── chapter.md
│   │   ├── drafts/
│   │   └── resources/
│   │
│   ├── 03-chapter-two/               # Chapter 3
│   │   ├── chapter.md
│   │   ├── drafts/
│   │   └── resources/
│   │
│   └── [continuing chapters...]
│
├── resources/                         # Shared resources (optional)
│   ├── images/                       # Global images
│   │   └── [shared images]
│   ├── research/                     # Research materials
│   │   ├── sources.md
│   │   └── [research documents]
│   ├── writing-samples/              # Your writing examples
│   │   └── persona-examples.md
│   └── templates/                    # Templates and examples
│       ├── chapter-template.md
│       └── writing-checklist.md
│
├── drafts/                            # Optional: working area for major revisions
│   └── [experimental drafts]
│
└── .gitignore                         # Git ignore file (optional)
```

---

## Chapter Folder Structure in Detail

Each chapter follows this consistent structure:

### `/book/NN-chapter-name/`
```
01-intro/
├── chapter.md              # Main, published chapter content
├── drafts/                 # Work-in-progress versions
│   ├── draft-v1-basic.md   # Initial draft
│   ├── draft-v2-expanded.md # Revised version
│   └── draft-v3-final.md   # Polish before publication
└── resources/              # Images, data, and supporting files
    ├── image-hero.png      # Hero image for chapter
    ├── diagram-one.svg     # Diagrams or graphics
    ├── chart-data.csv      # Data for charts
    └── sources.md          # Bibliography/sources for chapter
```

### Naming Conventions for Chapter Folders

- **Numbering**: Use 01, 02, 03... for sequential ordering
- **Descriptive names**: Include chapter topic: `01-introduction`, `02-getting-started`, `03-core-concepts`
- **Format**: Number-hyphen-lowercase-words: `05-advanced-techniques`
- **Avoid**: Special characters, spaces, or too-long names

### Examples
```
✅ Good:
- 01-introduction
- 02-getting-started
- 03-core-concepts
- 10-advanced-techniques
- 15-conclusion

❌ Avoid:
- Chapter 1
- introduction (no number)
- 1 intro (spacing/format)
- chapter_1_introduction (underscores)
- Ch1-IntroductionToTheTopic (too long/mixed case)
```

---

## File Organization Within Chapters

### Main Chapter File (`chapter.md`)
- Contains the final, published version of the chapter
- All structure, content, and style finalized
- Reviewed and approved
- This is the file that goes into the final book

### Drafts Folder (`drafts/`)
- Contains work-in-progress versions
- Each major iteration gets its own file
- Naming: `draft-v1-topic.md`, `draft-v2-topic.md`, etc.
- Keep drafts while revising, but clean up old versions before publishing
- Drafts are excluded from final book compilation

### Resources Folder (`resources/`)
- All images, diagrams, data files, and supporting materials
- Organized by type or topic
- Only committed to git if binary files are reasonable size
- Large files (videos, huge datasets) should be linked, not committed

---

## Resource File Naming

### Images
Use descriptive lowercase names with hyphens:
```
chapter-opening-image.png
hero-image-300x400.jpg
diagram-process-flow.svg
screenshot-example-001.png
```

### Data Files
```
data-survey-results.csv
chart-statistics-2024.json
research-sources.md
```

### Documents
```
sources-and-citations.md
research-notes.md
interview-transcript.md
```

---

## Shared Resources (Optional)

If your book uses many shared images or resources, create a global `/resources/` folder:

```
resources/
├── images/
│   ├── logo.png
│   └── common-diagrams/
├── research/
│   ├── sources.md
│   ├── interviews/
│   └── data/
├── writing-samples/
│   └── persona-examples.md
└── templates/
    ├── chapter-template.md
    └── section-template.md
```

Reference shared resources in chapters with relative paths:
```markdown
![Logo](../../resources/images/logo.png)
```

---

## Workflow Folder Organization

Some projects may benefit from additional organizational folders:

### `/drafts/` for Major Revisions
If you're experimenting with major restructuring:
```
drafts/
├── original-structure/         # Original chapter organization
├── alternate-structure-v1/     # Alternative organization
└── alternate-structure-v2/     # Another alternative
```

### `/outline/` for Planning Documents
```
outline/
├── book-structure.md           # Overall book outline
├── chapter-summaries.md        # Brief chapter summaries
└── timeline.md                 # Writing timeline/schedule
```

---

## Key Principles for Organization

### 1. One Chapter per Folder
Each chapter gets its own numbered folder. This makes it:
- Easy to locate specific chapters
- Clear which files belong together
- Simple to manage drafts and resources
- Straightforward to remove or reorder chapters

### 2. Separate Draft from Published
- `chapter.md` = final, published version
- `drafts/` = work-in-progress only
- Never edit drafts after publishing main chapter; update `chapter.md` instead
- This prevents confusion about which is the "real" version

### 3. Localize Resources
Keep chapter images and data in the chapter's `resources/` folder:
- Easier to manage and locate
- Clear what each chapter needs
- Simple to repurpose chapters
- Reduces clutter in repo root

### 4. Use Numbering Consistently
Sequential numbering (01, 02, 03...) ensures:
- Chapters appear in correct order
- Easy to see sequence at a glance
- Reordering chapters is straightforward
- Tools and scripts can sort correctly

### 5. Descriptive Names Add Context
Numbering alone isn't enough; include topic:
- `01-introduction` is clearer than `01`
- `05-advanced-techniques` explains chapter content
- Descriptive names aid navigation and understanding

---

## Moving and Reorganizing Chapters

### Reordering Chapters
1. Rename folders sequentially: `01-`, `02-`, `03-`, etc.
2. Update any cross-chapter links
3. Update book outline if you maintain one
4. Commit with message: "Reorder chapters [from]-[to]"

### Removing a Chapter
1. Delete the chapter folder
2. Renumber remaining chapters if needed
3. Update links and outline
4. Commit with message: "Remove chapter [number]: [topic]"

### Splitting a Chapter
1. Create new chapter folder with next available number
2. Move content from original chapter
3. Update both chapters with cross-references if needed
4. Commit with clear messages

### Merging Chapters
1. Combine content into one chapter
2. Delete the now-empty folder
3. Renumber remaining chapters
4. Commit with message: "Merge chapters [numbers]"

---

## .gitignore Configuration

For book projects, you might want to ignore:

```
# System files
.DS_Store
Thumbs.db

# Editor backups
*.swp
*.swo
*~

# Large files (if storing locally)
*.mp4
*.mov
*.psd

# Build/export artifacts
*.pdf
*.epub
*.docx
dist/
build/

# Node modules (if using tools)
node_modules/

# IDE settings (optional)
.vscode/
.idea/
```

---

## Size and Scalability

### Small Books (5-10 chapters)
- Simple structure works fine
- All chapters in `/book/`
- Shared resources in each chapter's `resources/`

### Medium Books (10-30 chapters)
- Structure still works
- Consider global `/resources/` for truly shared materials
- Maintain clear organization as book grows

### Large Books (30+ chapters)
- Consider organizing by part/section:
  ```
  book/
  ├── part-1-introduction/
  │   ├── 01-chapter/
  │   ├── 02-chapter/
  │   └── 03-chapter/
  ├── part-2-core-content/
  │   ├── 04-chapter/
  │   └── 05-chapter/
  └── part-3-conclusion/
      └── 06-chapter/
  ```

---

## Quick Reference

**Chapter Numbering**: 01, 02, 03... (leading zeros for clarity)

**Chapter Naming**: `01-descriptive-topic-name` (lowercase, hyphens)

**Files Per Chapter**:
- `chapter.md` (published version)
- `drafts/` folder (work-in-progress)
- `resources/` folder (images and data)

**Publishing**: Compile all `chapter.md` files from all chapters into final book

**Git Workflow**:
- Commit drafts as you work
- Finalize chapters to `chapter.md`
- Clean up old draft files before publishing
- Push to remote repository regularly

---

## Next Steps

See `/framework/process-write.md` for how to use this structure during the writing phase.
