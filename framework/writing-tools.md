# Writing Tools and Formats

This document describes the tools, formats, and technical conventions used for writing and managing your book project.

---

## File Format Standards

### Markdown (.md)
All book content is written in GitHub-flavored Markdown. This format:
- Is easy to read in plain text editors and on GitHub
- Converts cleanly to HTML, PDF, and other formats
- Allows version control and collaborative editing
- Works on any operating system

### File Naming Conventions
- Chapter files: `chapter.md` (main content for that chapter)
- Draft files: `draft-v1-topic.md`, `draft-v2-revised.md` (descriptive version numbers)
- Resources: Use lowercase with hyphens: `image-name.png`, `data-file.csv`
- Special characters: Avoid special characters in filenames; use hyphens for spaces

### File Organization
```
/book/
├── 01-intro/
│   ├── chapter.md          (main chapter content)
│   ├── drafts/             (work-in-progress versions)
│   │   ├── draft-v1-opening.md
│   │   └── draft-v2-revised.md
│   └── resources/          (images, data, references)
│       ├── image-hero.png
│       └── data-sources.md
├── 02-chapter-one/
├── 03-chapter-two/
└── [continuing chapters...]
```

---

## Markdown Formatting Reference

### Headings
```markdown
# Chapter Title (h1 - use once per chapter)
## Section Heading (h2 - main sections)
### Subsection (h3 - sub-topics within sections)
#### Minor Heading (h4 - rarely needed)
```

### Text Emphasis
```markdown
*italic text*           (use for titles, emphasis, internal thoughts)
**bold text**           (use for key concepts, important terms)
***bold italic***       (use sparingly for strong emphasis)
~~strikethrough~~       (rarely used, avoid unless necessary)
```

### Lists

#### Bullet Lists
```markdown
- Item one
- Item two
- Item three
  - Nested item
  - Another nested item
```

#### Numbered Lists
```markdown
1. First step
2. Second step
3. Third step
   1. Sub-step a
   2. Sub-step b
```

### Links
```markdown
[Link text](https://example.com)                    (external link)
[Link text](../01-intro/chapter.md)                 (relative link to another chapter)
[Link text](./resources/document.pdf)               (link to resource file)
```

### Images
```markdown
![Alt text for screen readers](./resources/image-name.png)
```

### Blockquotes and Callouts
```markdown
> Quote text here
> 
> — Attribution

> **Important Note:** This is a callout or important point
```

### Horizontal Line
```markdown
---
```

### Line Breaks
Single line breaks don't create new paragraphs in markdown. Use blank lines:
```markdown
Paragraph one.

Paragraph two.
```

---

## Special Formatting Elements

### Admonitions and Callouts
Use blockquotes for special callouts:

```markdown
> **Remember:** This is an important reminder
```

```markdown
> **Example:** Here is a specific example
```

```markdown
> **Key Point:** Central takeaway from this section
```

### Code Snippets
Inline code:
```markdown
Use `variable_name` for inline code references
```

Code blocks:
```markdown
\```python
# Python code example
def hello():
    print("Hello, World!")
\```
```

### Footnotes (if supported)
```markdown
This is a statement[^1]

[^1]: This is the footnote text
```

### Tables
```markdown
| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Data 1   | Data 2   | Data 3   |
| Data 4   | Data 5   | Data 6   |
```

---

## Writing Workflow with Version Control

### Using Git for Drafts
- Commit early and often with descriptive messages
- Use descriptive commit messages: "Draft opening section" not "update"
- Create branches for major revisions if needed
- Keep draft iterations organized in `/drafts/` folders

### Commit Message Examples
```
Add opening paragraph for chapter 2
Revise section 1.3 for clarity
Complete first draft of chapter 5
Polish dialogue in scene 3
Update examples in introduction
```

### Workflow: From Draft to Published
1. Create `draft-v1.md` and commit: "Initial draft of [topic]"
2. Revise and commit: "Revise draft for clarity"
3. Finalize to `chapter.md` and commit: "Complete chapter [number]"
4. Later revisions to `chapter.md` are incremental improvements

---

## Tools for Book Writing

### Essential Tools
- **Text Editor**: Use any markdown-friendly editor (VS Code, iA Writer, Markdown Editor, etc.)
- **Git**: For version control and tracking changes
- **GitHub/GitLab**: For hosting your repository
- **Claude Code**: This AI assistant for brainstorming, drafting, reviewing, and refining

### Optional Tools for Enhancement
- **Pandoc**: Convert markdown to PDF, Word, HTML, EPUB
- **Grammarly**: Grammar and spell-checking (use after first draft)
- **Hemingway Editor**: Readability analysis
- **Word frequency tools**: Identify overused words or patterns
- **Citation managers**: Track sources and generate bibliographies

---

## Export and Publication Formats

### From Markdown to Other Formats

#### PDF
```bash
pandoc chapter.md -o chapter.pdf
```

#### HTML
```bash
pandoc chapter.md -o chapter.html
```

#### Word (.docx)
```bash
pandoc chapter.md -o chapter.docx
```

#### EPUB (e-book)
```bash
pandoc chapter.md -o chapter.epub
```

### Compilation
To combine chapters into a single book:
```bash
pandoc 01-intro/chapter.md 02-chapter-one/chapter.md 03-chapter-two/chapter.md -o book.pdf
```

---

## Characters and Special Characters

### Common Markdown Issues
- Backslash escapes: Use `\` before special markdown characters if you need to display them literally: `\*`, `\[`, `\]`
- Curly quotes: Markdown supports "smart quotes" in most renderers
- Em dashes: Use `---` for em dashes (will render as —)
- Ellipses: Use `...` or `…`

### Characters to Use
```markdown
en dash (–): most contexts requiring a dash
em dash (—): for emphasis and interruptions
straight quotes: "like this"
smart quotes: "like this"
ellipsis (…): for trailing thoughts
```

---

## Editor Setup Recommendations

### VS Code Extensions (if using VS Code)
- "Markdown Preview Enhanced" for live preview
- "Markdown Linter" for consistent formatting
- "Spelling Checker" for spell-checking

### Write in Distraction-Free Mode
- Many editors have distraction-free modes
- Use full screen, dark mode, and focused view when writing
- Minimize notifications and other interruptions

---

## Accessibility Considerations

### For Readers
- Use descriptive alt text for all images
- Provide text alternatives for visual content
- Use proper heading hierarchy (don't skip levels)
- Ensure sufficient contrast and readability
- Use clear, simple language

### Alt Text Examples
```markdown
![A woman sitting at a coffee shop with a laptop and notebook](./resources/writing-scene.jpg)
```

Not: `![image]` or `![picture1]`

---

## Quick Reference: Markdown Cheat Sheet

| Element | Syntax |
|---------|--------|
| Heading 1 | `# Heading` |
| Heading 2 | `## Heading` |
| Bold | `**bold**` |
| Italic | `*italic*` |
| Link | `[text](url)` |
| Image | `![alt](url)` |
| Bullet list | `- item` |
| Numbered list | `1. item` |
| Blockquote | `> quote` |
| Code | `` `code` `` |
| Code block | ` ```code``` ` |

---

## Tips for Digital Writing

### Screen Readability
- Keep paragraphs shorter on screen than in print (3-5 sentences typical)
- Use section headers to break up content
- Use white space strategically
- Bold key concepts for scannability

### Working with Long Documents
- Write in focused sections (one chapter at a time)
- Organize with folder structure for easy navigation
- Use find-and-replace to maintain consistency
- Keep master outline updated as you write

### Backing Up Your Work
- Commit to git regularly (multiple times per writing session)
- Push to remote repository (GitHub) regularly
- Maintain local backups
- Never rely on a single copy

---

## Technical Troubleshooting

### Common Markdown Issues
**Problem**: Images aren't showing
- **Solution**: Check image path is relative and file exists. Use `./resources/image-name.png`

**Problem**: Links aren't working
- **Solution**: Verify file path and use relative paths: `../01-intro/chapter.md`

**Problem**: Formatting looks wrong in renderer
- **Solution**: Check for missing blank lines. Markdown requires blank lines between elements.

**Problem**: Apostrophes or quotes look wrong
- **Solution**: This is often a smart-quote vs. straight-quote issue. Most editors can normalize these.

---

## Next Steps

When you're ready to publish:
1. Ensure all chapters are finalized in `/book/`
2. Create a complete book file by combining all chapters
3. Export to desired format (PDF, EPUB, etc.)
4. Review formatted output for any display issues
5. Test links and images in final format

See `/framework/process-publish.md` for detailed publishing steps.
