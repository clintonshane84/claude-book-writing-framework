# Writing Rules and Best Practices

This document contains the rules and best practices for writing your book. It covers technical standards, craft techniques, and workflow processes to ensure quality, consistency, and readability throughout.

---

## Part 1: Technical Standards

### Markdown Format
- Use GitHub-flavored Markdown (.md extension) for all book content
- Structure chapters with headings: `# ` for chapter title, `## ` for sections, `### ` for subsections
- Use emphasis sparingly: **bold** for key terms, *italic* for emphasis or titles
- Use numbered lists for step-by-step content; bullet points for related items

### File Organization
- One chapter per folder: `/book/01-intro/`, `/book/02-chapter-one/`, etc.
- Main chapter content in `chapter.md`
- Work-in-progress drafts in `drafts/` subfolder
- Related images and resources in `resources/` subfolder
- Number chapters sequentially (01, 02, 03...) to maintain order

### Links and References
- Use relative paths for internal links: `[link text](../01-intro/chapter.md)`
- Link to resources: `![alt text](./resources/image-name.png)`
- Include source citations for external references
- Create bibliography for all sources (see skill-bibliography.md)

### Consistency Markers
- Define your book's key terms early and use them consistently
- Maintain consistent formatting for: chapter structures, section headers, callouts, examples
- Use consistent spacing: one blank line between paragraphs, two blank lines before major sections

---

## Part 2: Craft and Style

### Writing for Clarity
1. **Clear Subject**: Every sentence should have a clear subject and action
   - ✅ "The character walked through the door, noticing fresh flowers on the table."
   - ❌ "Walking through, fresh flowers were noticed."

2. **Active Voice Preference**: Use active voice unless passive voice serves a purpose
   - ✅ "Sarah discovered the hidden key" (clear, direct)
   - ❌ "The hidden key was discovered by Sarah" (passive, less direct)

3. **Concise Language**: Eliminate unnecessary words while preserving meaning
   - ✅ "She realized the truth" (4 words, clear)
   - ❌ "At that moment, it became clear to her that the truth was something she could no longer deny" (16 words, wordy)

4. **Concrete Over Abstract**: Use specific examples and details
   - ✅ "The coffee shop, with its worn leather chairs and jazz music, became her sanctuary"
   - ❌ "She liked going to places with atmosphere"

### Sentence Variety
- Vary sentence length: mix short, punchy sentences with longer, complex ones
- Avoid repetitive sentence structures on consecutive lines
- Use rhythm and pacing to control reader engagement
- Longer sentences for complex ideas; shorter sentences for impact

### Paragraph Structure
- Topic sentence first: start with the main idea
- Supporting sentences: develop and explain the idea
- Conclusion sentence: wrap up or transition
- Length: 3-5 sentences typical; vary as needed for pacing
- One idea per paragraph; don't overcrowd

### Voice and Tone
- Your persona defines your voice: the unique way you express ideas
- Maintain consistent tone throughout the book
- Adapt tone to audience (accessible vs. technical, formal vs. conversational)
- Let personality shine through: avoid generic or robotic writing
- Reference your persona-writing-style.md for specific guidance

### Show, Don't Tell
- Demonstrate through specific examples, dialogue, or scenes
- Avoid stating emotions directly; show them through action and detail
- ✅ "He clenched his fists, jaw tight" (shows tension)
- ❌ "He was angry" (tells, doesn't show)

### Dialogue and Interaction
- Dialogue should sound natural and reveal character
- Use dialogue tags sparingly: "said" often works best
- Vary dialogue with action and reflection
- Paragraph breaks for each speaker

---

## Part 3: Process and Workflow

### Writing Process Steps
1. **Draft First**: Get ideas on paper without perfectionism
2. **Revise for Structure**: Ensure paragraphs flow logically
3. **Revise for Clarity**: Simplify language, remove jargon
4. **Revise for Style**: Ensure voice is consistent with persona
5. **Edit Polish**: Fix grammar, punctuation, spelling

### Handling Drafts
- Work-in-progress drafts go in `drafts/` subfolder
- Keep drafts titled descriptively: `draft-v1-opening.md`, `draft-v2-revised.md`
- Use drafts to experiment without affecting main chapter file
- Move final version to `chapter.md` when ready

### Chapter Iteration
- Each chapter follows: Draft → Review → Revise → Final
- Review process uses skill-book-reviewing.md guidelines
- Revisions address: clarity, consistency, style, accuracy
- Multiple revision rounds are normal and expected

### Feedback and Revision
- When receiving feedback, address one type at a time (clarity, then style, then polish)
- Don't defend your first draft—revision makes it better
- Trust the revision process; most chapters improve dramatically in revision
- If stuck, take a break and return with fresh eyes

### Common Issues to Watch For
- **Passive voice overuse**: Scan for "was" and "were"; try active voice
- **Word repetition**: Don't repeat the same word in consecutive sentences
- **Vague pronouns**: Make sure every "it," "this," "that" refers clearly to something
- **Info dumps**: Spread exposition across multiple scenes/chapters rather than one block
- **Pacing problems**: Vary paragraph and sentence length to control reader speed
- **Inconsistent details**: Track names, dates, previous plot points for consistency

---

## Part 4: Quality Checkpoints

### Before Moving to Review
- [ ] Sentence is clear and makes sense when read aloud
- [ ] Paragraph has one main idea developed completely
- [ ] Section flows logically from previous section
- [ ] Tone matches your persona and established voice
- [ ] Technical accuracy verified (facts, names, dates)

### Style Consistency Check
- [ ] Terminology used consistently throughout chapter
- [ ] Formatting (headers, emphasis, lists) matches established patterns
- [ ] Tone aligns with persona-writing-style.md
- [ ] No unexplained jargon or terms readers won't understand
- [ ] Dialogue (if any) sounds natural and authentic

### Reader Experience Check
- [ ] Would a first-time reader understand this paragraph?
- [ ] Is there enough context, or does the reader need to backtrack?
- [ ] Does this sentence add value, or can it be cut?
- [ ] Would this detail interest or confuse a reader?
- [ ] Does the pacing feel right—too slow, too fast, or just right?

---

## Part 5: Special Formatting Guidelines

### Emphasis and Callouts
- Use **bold** for key concepts or important terms
- Use *italic* for book titles, emphasis, or internal thoughts
- Use blockquotes for extended quotes or important callouts:
  ```
  > "Your quote or callout here"
  ```

### Lists and Steps
- Use numbered lists for sequential steps
- Use bullets for parallel items (not in sequence)
- Introduce lists with a complete sentence ending in colon

### Code or Special Formatting
- Use backticks for inline code: `example_variable`
- Use triple backticks for code blocks with language specified:
  ~~~
  ```python
  code here
  ```
  ~~~

### Examples and Scenarios
- Clearly label examples: "Example:" or "For instance:"
- Use consistent formatting for scenarios or case studies
- When giving examples, explain the relevance to main text

---

## Part 6: Revision Checklist

Use this checklist during the review phase:

- [ ] **Content**: Does the chapter fulfill its purpose and cover intended topics?
- [ ] **Organization**: Do sections flow logically? Is there a clear structure?
- [ ] **Clarity**: Will readers understand the key points without confusion?
- [ ] **Voice**: Does the writing match the established persona and tone?
- [ ] **Consistency**: Are terms, details, and style consistent with the rest of the book?
- [ ] **Engagement**: Will this hold a reader's attention?
- [ ] **Length**: Is the chapter appropriate length—not too short or too long?
- [ ] **Grammar**: Are sentences grammatically correct and well-constructed?
- [ ] **Punctuation**: Is punctuation correct and used effectively?
- [ ] **Accuracy**: Are facts, references, and details accurate?

---

## Quick Reference

**Remember**:
- One idea, one paragraph
- Clear subject, active voice
- Show, don't tell
- Vary your sentence length
- Persona defines your voice
- Revision is where the magic happens
- Read your work aloud to catch awkward phrasing

**When you're stuck**:
- Take a break and return with fresh eyes
- Read the paragraph aloud; your ear will catch what your eyes miss
- Compare to your persona-writing-style.md; are you staying true to your voice?
- Ask: Does this sentence/paragraph serve the reader?
