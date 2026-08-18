# Resources and Assets Guide

This document explains how to manage images, diagrams, research materials, and other resources for your book project.

---

## Types of Resources

### 1. Visual Resources
- **Images**: Photographs, illustrations, screenshots
- **Diagrams**: Flow charts, process diagrams, mind maps
- **Charts/Graphs**: Data visualizations
- **Graphics**: Decorative or thematic artwork

### 2. Research Materials
- **Documents**: PDFs, research papers, articles
- **Data files**: CSV, JSON, or raw data
- **Interviews**: Transcripts or recordings
- **Statistics**: Datasets and sources

### 3. Supporting Content
- **Writing samples**: Examples of your persona
- **Reference materials**: Books, websites, documentation
- **Sources and citations**: Bibliography materials
- **Quotes**: Relevant quotes or excerpts to include

---

## Image Organization and Naming

### File Formats
**Recommended**:
- PNG: For graphics, diagrams, screenshots (lossless, good for web)
- JPG: For photographs (smaller file size, acceptable quality)
- SVG: For diagrams and graphics (scalable, best for diagrams)
- GIF: For simple animations (rare in books)

**Avoid**:
- BMP: Outdated, large file sizes
- TIFF: Large files, rarely needed for web/digital
- WebP: Not universally supported for e-readers

### Image Naming Convention
Use lowercase, descriptive names with hyphens:

```
chapter-topic-description-optional-version.extension

Examples:
✅ opening-scene-illustration.png
✅ process-flow-diagram-v2.svg
✅ character-portrait-sarah.jpg
✅ data-chart-revenue-2024.png
✅ screenshot-example-interface.png

❌ image1.png (not descriptive)
❌ Screenshot 2024-01-15 at 2.45.30 PM.png (too long, messy)
❌ final_REAL_version_use_this_one.png (unprofessional)
```

### Image Placement in Chapters
Store chapter-specific images in the chapter's resources folder:

```
/book/02-chapter-one/resources/
├── opening-illustration.jpg
├── key-diagram-process.svg
└── supporting-photo.png
```

Reference in chapter.md with relative paths:

```markdown
![Opening illustration for chapter](./resources/opening-illustration.jpg)
```

### Image Specifications

**For Web/Digital Viewing**:
- Resolution: 72-96 DPI
- Width: 600-800 pixels for chapter content
- File size: Keep under 500KB per image

**For Print Publishing**:
- Resolution: 300 DPI (minimum)
- Width: 1800-2400 pixels
- File size: Can be larger

**For Ebook (EPUB)**:
- Resolution: 100-150 DPI
- Width: 600-1000 pixels
- File size: Under 1MB per image

### Alt Text for Accessibility

Always include descriptive alt text for images:

```markdown
❌ ![image](./resources/photo.png)
❌ ![pic](./resources/photo.png)

✅ ![A woman sitting at a desk writing in a notebook](./resources/writing-scene.png)
✅ ![Diagram showing the relationship between planning, writing, review, and publish steps](./resources/process-flow.svg)
```

Good alt text:
- Describes what the image shows
- Explains why it's relevant to the chapter
- Is specific enough to be meaningful
- Isn't too long (under 125 characters ideal)

---

## Diagrams and Visual Elements

### Creating Diagrams
**Tools**:
- Lucidchart: Professional diagrams (web-based)
- Draw.io: Free, open-source diagram tool
- OmniGraffle: Mac-based, professional
- Figma: Modern design tool
- Canva: Simple templates and graphics

### Diagram Formats
**SVG** (Scalable Vector Graphics):
- Best for diagrams, charts, process flows
- Scales without quality loss
- Smaller file sizes than raster
- Can be edited and updated easily

**PNG**:
- Good for screenshots and diagrams
- Lossless quality
- Larger than SVG for diagrams
- Better for complex illustrations

### Embedding Diagrams in Markdown

```markdown
![Process Flow Diagram](./resources/process-flow.svg)

![Screenshot of the interface](./resources/screenshot.png)
```

---

## Data and Statistics

### Data File Organization

```
/book/chapter-folder/resources/
├── chapter.md
├── data/
│   ├── survey-results.csv
│   ├── interview-summaries.json
│   └── statistics-2024.xlsx
└── research/
    └── sources.md
```

### Data File Formats
- **CSV**: Comma-separated values (spreadsheet data)
- **JSON**: Structured data (good for nested information)
- **XLSX**: Excel spreadsheet (if you need formulas)
- **MD**: Markdown table or formatted text

### Referencing Data
In your chapter, reference the data clearly:

```markdown
## Survey Results

According to our 2024 survey of 500 respondents:
- 78% reported increased satisfaction
- 22% reported no change

*See `resources/data/survey-results.csv` for full dataset*
```

### Source Documentation

Create a `sources.md` file in each chapter's resources:

```markdown
# Sources for Chapter 2: Getting Started

## Survey Data
- 2024 User Survey
- Conducted: January-February 2024
- Sample size: 500 respondents
- File: `survey-results.csv`

## Interviews
- Interview with Sarah Chen, Oct 2024
- Interview with Marcus Johnson, Nov 2024
- Files in `interviews/` folder

## Research
- "The Study of Effectiveness" (Smith, 2023)
- Link: https://example.com/study
- Pages referenced: 45-67
```

---

## Research Materials

### Organizing Research
```
/resources/research/
├── sources.md                    # Master source list
├── research-by-topic/
│   ├── topic-1/
│   │   ├── notes.md
│   │   └── sources.md
│   └── topic-2/
│       ├── notes.md
│       └── sources.md
└── interviews/
    ├── interview-1-transcript.md
    ├── interview-2-transcript.md
    └── interview-notes.md
```

### Citation Management
Maintain a master bibliography/sources file:

```markdown
# Bibliography and Sources

## Books
- Author Name. "Book Title." Publisher, Year.
- Author Name. "Book Title." Publisher, Year.

## Websites
- Website Title. URL. Accessed: Date.
- Website Title. URL. Accessed: Date.

## Interviews
- Interview with Name, Date
- Interview with Name, Date

## Research Papers
- Author. "Paper Title." Journal, Year.
```

---

## Writing Samples and Persona Examples

### Organizing Persona Examples

```
/resources/writing-samples/
├── persona-examples.md          # All your writing examples
├── example-1-conversational.md  # One example per file (optional)
├── example-2-emotional.md       # Shows different aspects of voice
└── example-3-instructional.md   # Teaching voice example
```

### Sample Format

```markdown
# Your Writing Samples

## Sample 1: Opening with Personal Story
[Your sample text here - 3-5 paragraphs showing your voice]

Author's Note: This sample shows my conversational tone and use of personal anecdotes.

## Sample 2: Emotional/Vulnerable Writing
[Your sample text here showing vulnerability or deep feeling]

Author's Note: This demonstrates how I handle emotion and create intimacy with readers.

## Sample 3: Instructional/Teaching Voice
[Your sample text here showing how you explain concepts]

Author's Note: This shows my teaching voice and how I make complex ideas accessible.
```

---

## External Resources and Links

### Linking to External Resources
For large files or external materials, link rather than commit:

```markdown
## Additional Resources

- Full dataset: [Download from link](https://example.com/data)
- Supporting paper: [Read online](https://example.com/paper.pdf)
- Video interview: [Watch on YouTube](https://youtube.com/...)
```

### Storing URLs and References
Create a `resources.md` file at project level:

```markdown
# External Resources

## Research Links
- Topic 1: https://example.com/research-1
- Topic 2: https://example.com/research-2

## Inspirations
- Similar books: [Title](link)
- Related articles: [Title](link)

## Tools and Utilities
- Markdown editor: [Tool name](link)
- Image optimizer: [Tool name](link)
```

---

## File Size and Git Considerations

### Managing Large Files
**Keep in repository**:
- Text files (MD, CSV)
- Small images under 500KB
- SVG diagrams
- Typical project resources

**Consider external storage**:
- Video files
- Large datasets (>10MB)
- High-resolution image archives
- Historical versions you want to keep but not in active branch

### Using .gitignore
```
# Ignore large files
*.mp4
*.mov
*.psd
*.zip

# Ignore build artifacts
*.pdf
dist/
build/

# Ignore system files
.DS_Store
Thumbs.db
```

---

## Updating and Versioning Resources

### Managing Updated Resources
If you update an image or data file:

```
Version 1:
chapter-diagram.svg

Version 2:
chapter-diagram-v2.svg

OR

chapter-diagram.svg (replace and commit with message: "Update chapter diagram for clarity")
```

Choose one approach consistently:
- **Version suffix** (`-v1`, `-v2`) if you need history
- **Replace in place** if you don't need to keep old versions

### Committing Resource Changes
```bash
git add resources/
git commit -m "Add images and data for chapter 2"

git add resources/chapter-diagram.svg
git commit -m "Update diagram for section 2.3 for clarity"
```

---

## Best Practices for Resources

1. **Name clearly**: Descriptive names make files easy to find
2. **Organize locally**: Keep chapter resources with chapter folders
3. **Document sources**: Always note where images/data come from
4. **Provide alt text**: Ensure images are accessible
5. **Optimize files**: Use appropriate formats and compression
6. **Link externally**: For very large files, link instead of storing
7. **Keep it organized**: Consistent structure throughout project
8. **Update thoughtfully**: Commit resource changes with clear messages

---

## Checklist for Resources

Before publishing each chapter:

- [ ] All images have descriptive alt text
- [ ] Image files are optimized (appropriate size and resolution)
- [ ] Image paths are relative and correct
- [ ] Data files are organized in resources folder
- [ ] Sources for all data and quotes are documented
- [ ] External links are verified and working
- [ ] Image file names are descriptive and consistent
- [ ] All diagrams are clear and properly labeled
- [ ] Resource organization matches project structure

---

## Next Steps

See `/framework/process-write.md` for guidance on integrating resources while writing chapters.
