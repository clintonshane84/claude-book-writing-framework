# Phase 2: Writing Process

The Writing phase is where you actually draft the chapters of your book. This is the core creative work where content comes to life, following the outline created in Phase 1.

**Duration**: Varies by book size (1-6+ weeks depending on chapter count and writing pace)

**Outcome**: Complete drafts of all chapters following your persona and writing style

---

## Phase 2 Overview

The Writing phase works through your book chapter by chapter:

1. **For Each Chapter**: Follow the chapter writing workflow
2. **Maintain Consistency**: Keep chapters aligned with persona and outline
3. **Build Momentum**: Write systematically through all chapters
4. **Draft First**: Prioritize getting words on page over perfection

---

## Chapter Writing Workflow

Each chapter follows this core workflow:

### Step 1: Prepare the Chapter
Before writing, gather everything you need

**Checklist**:
- [ ] Chapter outline available (from Phase 1)
- [ ] Research materials gathered
- [ ] Related writing samples reviewed (for voice reference)
- [ ] persona-writing-style.md reviewed as reminder
- [ ] Resources (images, data) identified
- [ ] `/book/NN-chapter-name/chapter.md` file created and open

**Duration**: 10-15 minutes

### Step 2: Draft the Chapter
Write the chapter from start to finish

**Process**:
1. **Write opening**: Hook the reader, introduce the chapter topic
2. **Write main content**: Develop each section/point from outline
3. **Add examples**: Illustrate concepts with stories, case studies, or examples
4. **Write closing**: Summarize key points, bridge to next chapter
5. **Don't edit yet**: Get the full draft written before revising

**Key reminders**:
- Follow the chapter outline as guide (not rigid structure)
- Refer to persona-writing-style.md to maintain voice
- Include specific examples and details
- Aim for target word/page count
- Write with reader in mind

**Duration**: 1-3 hours depending on chapter length and complexity

### Step 3: Self-Review the Chapter
Read through the draft and assess quality

**Self-review checklist**:
- [ ] **Clarity**: Does each paragraph make sense? Would a reader understand it?
- [ ] **Structure**: Do sections flow logically? Is there a clear progression?
- [ ] **Voice**: Does this sound like you? Does it match persona?
- [ ] **Completeness**: Did you cover all outline points? Anything missing?
- [ ] **Examples**: Are there enough specific examples and details?
- [ ] **Length**: Does it match target length? Too short/long?

**Make quick fixes**:
- Reorder sections if flow is awkward
- Add missing content from outline
- Remove redundant paragraphs
- Clarify confusing sentences
- Strengthen weak transitions

**Don't obsess over**:
- Grammar and spelling (fix later in review phase)
- Perfect word choice (revision will improve)
- Punctuation details (polish phase handles this)

**Duration**: 30-45 minutes

### Step 4: Commit Chapter
Save your work to git

**Process**:
1. Save all changes to `chapter.md`
2. Stage changes: `git add book/NN-chapter-name/`
3. Commit with message: `git commit -m "Draft chapter NN: Chapter Title"`
4. Push to remote: `git push origin main`

**Message examples**:
```
Draft chapter 01: Introduction
Draft chapter 05: Core Strategies
Complete chapter 08: Application and Practice
```

**Duration**: 5 minutes

---

## Maintaining Consistency Across Chapters

### Style and Tone Consistency

**Each chapter should**:
- Use consistent vocabulary and terminology
- Maintain established tone (friendly, formal, conversational, etc.)
- Follow narrative approach (stories, examples, analysis, etc.)
- Match sentence structure patterns
- Use consistent emphasis and formatting

**Consistency checks**:
- Refer to persona-writing-style.md before each chapter
- Reread previous chapters occasionally to stay in voice
- Keep list of key terms used consistently
- Note any character names or recurring references
- Track patterns in your own writing

**If you drift from established voice**:
- This is normal—writing voice shifts slightly per session
- Use review phase to catch and correct inconsistencies
- Can adjust persona-writing-style.md if your voice naturally evolved

### Continuity and Threading

**Connect chapters together**:
- Each chapter should reference or build on previous chapters
- Introduce concepts progressively (don't assume knowledge)
- Provide context when referring back
- Create bridges between chapters

**Example bridge from Chapter 2 to Chapter 3**:
```
In Chapter 2, we explored the foundation of effective planning. 
Now that you understand the core principles, Chapter 3 builds on 
that foundation to show you how to implement these principles in 
your own life.
```

### Reference Management
Keep track of important details for consistency:

**Create a reference doc** at `/resources/consistency-tracking.md`:
```markdown
# Consistency Tracking

## Characters/People Referenced
- Sarah (introduced Ch. 2, example of success)
- Marcus (introduced Ch. 5, represents challenge)

## Key Statistics/Data
- 78% satisfaction rate (from 2024 survey, Ch. 3)
- Founded in 2020 (organization, mentioned Ch. 1)

## Terminology
- "Growth mindset" - consistent term throughout
- "Strategic planning" vs. "tactical planning" - distinct terms

## Chapter Connections
- Ch. 1 introduces X → Ch. 2 builds on X → Ch. 3 applies X
- Ch. 4 references story from Ch. 2
```

---

## Handling Writing Challenges

### Stuck on a Section?

**If you can't write a particular section**:
1. **Skip it**: Mark with `[TODO: section name]` and move on
2. **Write it differently**: Try a different approach (story vs. explanation)
3. **Review source**: Check research/outline for missing pieces
4. **Take a break**: Sometimes stepping away helps
5. **Simplify**: Remove requirements; just capture the core idea

**Example**:
```markdown
## Section: Advanced Techniques
[TODO: Expand on technique 3 with real-world example]

For now:
- Technique 1: [written]
- Technique 2: [written]
- Technique 3: [summary only - needs full treatment]
- Technique 4: [written]
```

### Chapter Feels Too Short or Long?

**Too short** (under target):
- Add more examples or stories
- Expand explanations with more detail
- Include additional supporting points
- Add examples of what NOT to do

**Too long** (over target):
- Is there a section that doesn't serve the chapter's purpose? Cut it.
- Can any points be condensed?
- Are there redundant examples?
- Should a large section be moved to next chapter?

### Voice Shifting or Inconsistent?

**If chapter sounds different from others**:
- Review persona-writing-style.md
- Reread opening of previous chapter
- Identify specific differences (sentence length, vocabulary, tone)
- Revise to bring back consistency

Example: If Chapter 1 uses short sentences but Chapter 4 has long run-ons:
```
Read Ch. 1 opening: "Short sentences. Direct. Clear."
Read Ch. 4 opening: "Long, flowing sentences that build meaning through..."
→ Revise Ch. 4 to match Ch. 1's rhythm
```

---

## Workflow: Write Multiple Chapters

When writing sequential chapters:

### Daily Writing Session
```
1. Review previous chapter's final version (5 min)
2. Read outline for current chapter (5 min)
3. Draft chapter (1-2 hours)
4. Self-review (30 min)
5. Commit to git (5 min)
```

### Multi-Day Writing for One Chapter
If a chapter takes multiple days:

**Day 1**:
- Draft sections 1-3
- Commit: "Draft chapter sections 1-3"

**Day 2**:
- Draft remaining sections
- Do self-review
- Commit: "Complete draft chapter XX"

**Day 3**:
- Revisions based on review
- Final check
- Commit: "Polish chapter XX - ready for review phase"

### Weekly Progress

**Example week plan** (5 chapters per week):
```
Mon: Draft Ch. 1
Tue: Draft Ch. 2
Wed: Draft Ch. 3
Thu: Draft Ch. 4
Fri: Draft Ch. 5
Weekend: Catch-up and revisions
```

---

## Tips for Productive Writing

### Before You Write
- **Eliminate distractions**: Phone off, browser closed, quiet space
- **Warm up**: Read related writing samples or outline first
- **Set a timer**: 90-minute focused sessions work well
- **Clear goal**: Know what chapter/section you'll complete today

### While Writing
- **Write fast**: Aim for momentum, not perfection
- **Follow the outline**: Use it as map, not straitjacket
- **Trust the process**: First draft is always rough; that's normal
- **Show, don't tell**: Use examples and stories, not just explanation
- **Write for your reader**: Imagine them reading this chapter

### After Writing
- **Take a break**: Step away before self-review
- **Read aloud**: Your ear catches what eyes miss
- **Commit early**: Don't wait to perfect before committing to git
- **Celebrate**: Completing a chapter is a big deal!

---

## Managing Chapters and Organization

### Chapter File Management

Keep chapters organized:
```
/book/01-intro/
├── chapter.md          (main published version)
├── drafts/
│   ├── draft-v1.md     (initial draft)
│   └── draft-v2.md     (revisions)
└── resources/
    ├── images/
    └── data/
```

**Process**:
1. Write initial draft in `chapter.md`
2. Save backup to `drafts/draft-v1.md` when done
3. If major revision needed, save to `drafts/draft-v2.md`
4. Keep final version in `chapter.md`

### Using Skills During Writing

**Available skills for writing phase**:
- **skill-book-writing.md**: Draft chapters, develop ideas, improve prose
- **skill-chapter-organization.md**: Structure chapters, improve flow
- **skill-book-research.md**: Find supporting information or data
- **skill-content-editing.md**: Refine language, strengthen writing

---

## Writing Cycle: Multiple Passes

Some projects benefit from multiple passes through the book:

### First Pass (Rough Draft)
- Get all content written quickly
- Rough structure is okay
- Don't worry about perfection
- Focus on completion

### Second Pass (Structure)
- Reorder sections if needed
- Ensure clear progression
- Add missing content
- Remove redundant content

### Third Pass (Voice and Style)
- Ensure consistent tone
- Align with persona
- Improve sentence variety
- Strengthen examples

### Fourth Pass (Polish)
- Fix grammar and spelling
- Perfect punctuation
- Final proofreading
- Ready for review phase

---

## Chapter Writing Checklist

Use this checklist for each chapter:

**Preparation**:
- [ ] Outline reviewed
- [ ] Research gathered
- [ ] Resources identified
- [ ] Previous chapters reviewed for continuity
- [ ] Persona-writing-style.md reviewed

**Writing**:
- [ ] Opening hooks reader
- [ ] All outline sections covered
- [ ] Examples provided
- [ ] Transitions between sections smooth
- [ ] Closing summarizes and bridges to next chapter
- [ ] Target word/page count achieved

**Self-Review**:
- [ ] Clarity: Would reader understand?
- [ ] Flow: Does it progress logically?
- [ ] Voice: Matches established persona?
- [ ] Completeness: Nothing major missing?
- [ ] Examples: Sufficient detail and illustration?

**Commit**:
- [ ] Changes saved to chapter.md
- [ ] Committed to git with clear message
- [ ] Pushed to remote repository

---

## Common Writing Phase Mistakes to Avoid

- ❌ **Perfecting early**: First draft doesn't need to be perfect
- ❌ **Over-explaining**: Trust reader; let examples speak
- ❌ **Losing voice**: Check persona mid-chapter if it feels off
- ❌ **Ignoring outline**: Outline is guide, not prison, but use it
- ❌ **Forgetting continuity**: Reference previous chapters to build understanding
- ❌ **Trying too hard**: Best writing comes from natural flow, not forcing
- ❌ **No git commits**: Commit work regularly to avoid losing progress

---

## Signs Phase 2 is Complete

✅ **Writing phase is complete when**:
- All chapters have been drafted
- Each chapter has been through self-review
- All chapters follow persona and style
- Chapters are organized in `/book/` structure
- Chapter continuity and references are clear
- All changes are committed and pushed to git
- You're ready to move to Phase 3 (Review)

---

## Next Phase

Once all chapters are drafted and committed:
→ Move to `/framework/process-review.md` for Phase 3: Review

This phase guides you through editing, refining, and polishing each chapter for quality and consistency.
