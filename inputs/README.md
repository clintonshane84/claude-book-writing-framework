# Global Inputs and Resources

This folder contains global resources and materials for your entire book project. These files are automatically available to Claude when writing chapters and should inform the content development across all chapters.

## What Goes Here

Use the three subfolders to organize your book's global materials:

### 📝 `draft-pages/` - Partially Written Content

Place any existing chapter drafts, partial pages, or rough outlines that should inform the book writing:

- Already-written opening paragraphs or sections
- Partial chapters you want Claude to expand or complete
- Rough notes or outlines for entire chapters
- Key passages you've already written and want to preserve
- Previous versions or attempts at chapters

**Example**:
```
draft-pages/
├── chapter-1-opening.md
├── chapter-5-rough-draft.md
└── opening-thoughts.md
```

### 🔍 `research/` - Research Materials and Findings

Place research documents, reports, and findings that support your book content:

- Research papers and articles
- Survey results and data
- Interview transcripts
- Case studies and examples
- Industry reports and statistics
- Literature review notes
- Scientific studies
- Historical documentation

**Example**:
```
research/
├── 2024-productivity-study.md
├── interview-transcripts.md
├── market-research-findings.pdf
└── statistical-analysis.md
```

### 📚 `references/` - Reference Materials and Inspiration

Place reference books, examples, and inspiration materials:

- Excerpts from relevant books
- Similar book outlines or structures
- Examples of writing in your style
- Industry-specific terminology guides
- Visual examples or diagrams explained
- Quotes or passages for inspiration
- Competitor or similar book analysis

**Example**:
```
references/
├── similar-books-analysis.md
├── writing-style-examples.md
├── technical-terminology.md
└── inspirational-passages.md
```

## How Claude Uses These Files

When you use the **skill-book-writing.md** to draft chapters:

1. **Automatic Context**: Claude automatically reads and includes all files in `/inputs/` as context when writing
2. **Seamless Integration**: Research and draft materials inform the writing naturally
3. **Content Continuity**: Partially-written content guides the completion of chapters
4. **Reference Material**: Examples and references provide style and structure guidance
5. **Data Integration**: Statistics and findings are woven into chapter content

You don't need to manually reference these files—Claude automatically considers them.

## Organization Tips

### For Drafts
- Name files clearly: `chapter-01-draft.md`, `introduction-partial.md`
- Include dates if you have multiple versions: `chapter-03-v1.md`, `chapter-03-v2.md`
- Note what's complete and what needs finishing

### For Research
- Organize by topic or chapter: `chapter-2-research/`, `background-research/`
- Include source citations in files
- Summarize key findings at the top of each file
- Note which chapters each research item applies to

### For References
- Keep one file per reference type: `writing-examples.md`, `structure-examples.md`
- Include clear labels: `## Example 1: Opening Hook`, `## Example 2: Narrative Flow`
- Note why each reference is included and how it should influence writing

## Before Starting to Write

**Before using skill-book-writing.md to draft chapters**:

1. ✅ Organize any existing materials into this folder
2. ✅ Create clear filenames that explain the content
3. ✅ Add brief descriptions at the top of each file
4. ✅ Ensure research and drafts are in appropriate subfolders
5. ✅ Commit these files to git

**When you're ready to write chapters**:
- All materials in `/inputs/` will be available to Claude automatically
- No need to paste content repeatedly—Claude will reference as needed
- The framework ensures consistency with your existing materials

## Examples

See the example files in each subfolder to understand the expected format and content type.

## What NOT to Put Here

- ❌ Personal notes you don't want to influence writing
- ❌ Outdated or wrong information
- ❌ Very large files (commit separately or reference)
- ❌ Binary files (images/PDFs) - reference in the research/reference markdown files instead
- ❌ Content that contradicts your book's direction

## Updating During Writing

You can add more materials to `/inputs/` at any time:
- If you find new research while writing, add it here
- If you realize something should influence all chapters, put it here
- If inspiration strikes between chapters, capture it here

Claude will automatically consider new additions when writing subsequent chapters.

## Tips for Best Results

### Be Specific in References
```
Good: "Use the structure from chapter 3 in 'Atomic Habits': Hook → Insight → Practice"
Better: See references/atomic-habits-structure.md for detailed breakdown
```

### Organize Research by Relevance
```
research/
├── core-concept-1-research.md
├── core-concept-2-research.md
└── supporting-evidence.md
```

### Complete Your Drafts
```
draft-pages/
├── chapter-1-opening.md (Ready for expansion - has hook and first section)
└── chapter-5-notes.md (Just notes - needs full drafting)
```

## Questions?

Refer to:
- `/framework/directory-structure.md` - Detailed structure guidelines
- `/framework/process-write.md` - How global inputs are used during writing
- `/framework/skills/skill-book-writing.md` - How Claude uses these materials

Your `/inputs/` folder is where your book's foundation lives. The more complete and organized these materials are, the better Claude can write chapters that build on them.

---

**Remember**: The files in this folder automatically become context for chapter writing. Keep them relevant, organized, and updated!
