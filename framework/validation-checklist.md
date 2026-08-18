# Pre-Writing Validation Checklist

Before starting the book writing process, this expanded validation checklist ensures all necessary inputs, resources, and clarifications are in place. Claude must verify each item and ask clarifying questions if anything is missing or unclear.

---

## Phase 0: Validation and Preparation

### Before Claude Begins Any Work

This is a **required checkpoint**. Claude should not proceed to Phase 1 (Plan) until all items below are validated.

---

## Section 1: Existing Book Drafts

**Status**: [ ] Complete - [ ] Partial - [ ] Not Started

### 1.1 Book Page Drafts
- [ ] **At least one page/chapter draft exists**
  - Complete draft is ideal
  - Partial draft is acceptable
  - Draft should show intended direction and style
  
**Questions to ask if missing**:
- Do you have any partial chapters or pages already written?
- Have you outlined the basic structure and chapters?
- Do you have rough notes or ideas you'd like to refine?

**Action if provided**:
- Read all existing drafts
- Understand what's been written and what needs to be written
- Note any patterns in style or structure

### 1.2 Scope and Coverage
- [ ] **Book covers a clear topic or story**
- [ ] **Intended chapter count is defined** (or approximate)
- [ ] **Book length goal is stated** (number of pages/words, or "complete manuscript")

**If missing, ask**:
- What is the central topic or story this book covers?
- How many chapters do you envision?
- What's your target length (number of pages or chapters)?

---

## Section 2: Writing Persona and Style

**Status**: [ ] Complete - [ ] Partial - [ ] Need to Extract

### 2.1 Writing Examples from Author
- [ ] **1-2 page samples of YOUR writing provided**
  - These should be existing work, not examples from others
  - At least 2-3 paragraphs minimum (ideally full pages)
  - Can be from different contexts (blog, journal, previous work, etc.)

**If missing, ask**:
- Can you provide 1-2 examples of your writing (from blog, journal, previous work)?
- What pieces best represent how you naturally write?
- If you don't have existing examples, are you willing to write a sample page now?

### 2.2 Persona and Voice Elements
The author should provide or confirm:

- [ ] **Tone/Voice descriptor**: (conversational, formal, warm, analytical, humorous, etc.)
- [ ] **Target audience**: (age group, experience level, what they're seeking)
- [ ] **Book genre/category**: (self-help, fiction, educational, memoir, etc.)
- [ ] **Writing style preferences**: 
  - Sentence length (short and punchy vs. flowing)
  - Use of anecdotes, examples, or stories
  - Level of formality

**If persona information is sketchy or missing**:
1. Ask the author clarifying questions
2. Extract persona from their writing examples
3. Document findings in persona-writing-style.md
4. Have author review and confirm it accurately represents them

### 2.3 Content and Themes
- [ ] **Main themes of the book are clear** (3-5 central ideas)
- [ ] **Book's purpose is stated**: What will readers gain/learn/experience?
- [ ] **Any specific style requirements are noted** (story-driven, example-heavy, etc.)

**Questions to clarify**:
- What are the central themes or big ideas in this book?
- What should readers take away or gain from it?
- How important are stories/examples vs. explanation?

---

## Section 3: Resources and Reference Materials

**Status**: [ ] Complete - [ ] Partial - [ ] Not Needed

### 3.1 Global Resources in `/inputs/` Folder
- [ ] **Global resources organized** (if applicable to this book)
  - Partially written draft pages/chapters
  - Research reports, findings, and studies
  - Reference materials and examples
  - Supporting documents for entire book

**If applicable, verify**:
- [ ] `/inputs/` folder exists and is organized
- [ ] Draft pages available in `/inputs/draft-pages/`
- [ ] Research materials organized in `/inputs/research/`
- [ ] Reference materials organized in `/inputs/references/`
- [ ] All global resources are committed to git

**If needed for this book, ask**:
- Do you have partially written chapters or draft pages to provide?
- Are there research reports, studies, or findings this book will reference?
- Do you have reference materials (examples, templates, inspiration) to share?
- Can you organize and upload these to `/inputs/` before we begin writing?

**Note**: Claude will automatically use all files in `/inputs/` as context when writing chapters, so ensuring these are comprehensive and well-organized will improve chapter quality.

### 3.2 Source Materials
- [ ] **Research materials are available or accessible**
  - Books, articles, studies to reference
  - Data or statistics to include
  - Interview transcripts or notes
  - External resources or links

**If missing, ask**:
- Do you have research materials to support the content?
- Are there specific sources you want to cite?
- Do you have data, statistics, or studies to reference?
- Can these materials be linked if not stored locally?

### 3.3 Supporting Documents
- [ ] **Outline or structure document** (optional but helpful)
  - Chapter-by-chapter outline
  - High-level structure
  - Main points per chapter

### 3.4 Images and Visual Assets
- [ ] **Images/graphics identified** (if needed)
  - List of images to create or source
  - Descriptions of needed diagrams
  - Locations where visuals should appear

**If applicable, ask**:
- Will this book include images or diagrams?
- Where should images appear?
- Do you have images, or do they need to be created?

---

## Section 4: Clarifying Questions and Assumptions

### 4.1 Book Scope and Structure
- [ ] **What is the book about?** (in 1-2 sentences)
- [ ] **How many chapters will it have?** (approximate number)
- [ ] **What's the intended length?** (pages, words, or completion scope)

### 4.2 Writing Approach
- [ ] **Should the book be story-driven or concept-driven?**
- [ ] **How much personal experience should be included?**
- [ ] **What's the relationship with the reader?** (teacher, friend, expert, guide, peer)

### 4.3 Timeline and Goals
- [ ] **When do you want the book completed?** (or chapter-by-chapter timeline)
- [ ] **Any deadlines or milestones?**
- [ ] **How frequently should writing happen?** (daily, weekly, as-needed)

### 4.4 Special Considerations
- [ ] **Any chapters or sections already drafted that should be preserved as-is?**
- [ ] **Any topics that are sensitive or require special care?**
- [ ] **Any stylistic requirements or constraints?** (must avoid certain terms, formats, etc.)

---

## Section 5: Persona Documentation

### 5.1 Persona File Created
- [ ] **persona-writing-style.md exists**
- [ ] **File includes**:
  - Your writing voice description
  - Target audience
  - Book genre and purpose
  - Core themes
  - Tone and formality level
  - Sentence and paragraph style
  - Vocabulary level
  - Narrative approach
  - Examples of your writing
  - Consistency guidelines

### 5.2 Persona Accuracy
- [ ] **Author has reviewed persona-writing-style.md**
- [ ] **Author confirms it accurately represents their voice**
- [ ] **Author has provided feedback or corrections** (if needed)
- [ ] **Persona file has been updated** based on feedback

**If persona document needs creation or revision**:
1. Extract voice from author's writing examples
2. Ask clarifying questions about the points above
3. Create persona-writing-style.md draft
4. Have author review and provide feedback
5. Finalize persona document

---

## Section 6: Framework Setup

### 6.1 Repository Structure
- [ ] **/framework/ folder exists** with all framework files
- [ ] **/book/ folder exists** (empty, ready for content)
- [ ] **CLAUDE.md file is present** (main orchestration file)
- [ ] **README.md file is present** (project overview)

### 6.2 Chapter Folders Created
- [ ] **At least one chapter folder started** (e.g., `/book/01-intro/`)
- [ ] **chapter.md file exists** (for main content)
- [ ] **drafts/ folder exists** (for work-in-progress)
- [ ] **resources/ folder exists** (for images/data)

---

## Section 7: Final Confirmation Checklist

Before proceeding to Phase 1 (Plan), confirm:

- [ ] **✅ Book topic/story is clear**
- [ ] **✅ At least one draft page or outline exists**
- [ ] **✅ Writing examples provided and analyzed**
- [ ] **✅ Persona-writing-style.md is complete and confirmed**
- [ ] **✅ Target audience is defined**
- [ ] **✅ Book scope (chapters, length) is clear**
- [ ] **✅ Resources/materials are available or linked**
- [ ] **✅ No blocking questions remain unanswered**
- [ ] **✅ Author is ready to move forward**
- [ ] **✅ Framework folders and files are set up**

---

## Validation Outcome

### ✅ If All Items Are Complete

**Status**: VALIDATED - Ready to proceed to Phase 1 (Planning)

**Next steps**:
1. Confirm with author: "All inputs are validated. Ready to move to the Planning phase."
2. Move to `/framework/process-plan.md`
3. Begin Phase 1: Plan (book structure, chapter outline, writing targets)

### ⚠️ If Some Items Are Missing or Unclear

**Status**: PENDING - Request additional information

**Next steps**:
1. List what's missing or needs clarification
2. Ask specific questions (use AskUserQuestion if needed)
3. Wait for author responses
4. Update validation checklist as items are provided
5. Re-check; proceed when all items are complete

### ❌ If Critical Items Are Missing

**Status**: NOT READY - Cannot proceed without critical inputs

**Critical items** (must have):
- Book topic is defined
- At least one draft or outline exists
- Writing examples or persona information
- Target audience is clear

If these critical items are missing:
1. Explain what's needed to proceed
2. Suggest: "Let's start by understanding your book better" or "Can you share a sample of your writing?"
3. Work with author to gather minimum viable inputs
4. Re-attempt validation

---

## Detailed Validation Conversation Flow

### Step 1: Greet and Explain Validation
```
Welcome! Before we begin writing your book, I need to verify a few things to ensure 
we have everything needed for a successful writing process. This usually takes 10-15 
minutes and ensures we're aligned on your book's scope, your writing style, and the 
resources we'll need. Let's start!
```

### Step 2: Assess What Exists
```
First, let me understand what you already have:
- Do you have any draft chapters or pages started?
- Have you written any samples that show your writing style?
- Do you have an outline or structure in mind?
```

### Step 3: Extract Persona
If no existing persona document:
```
I'd like to understand your unique writing voice. Can you share 1-2 examples of 
your writing (from a blog, previous work, journal, etc.)? Even 2-3 paragraphs would 
be helpful. If you don't have existing samples, I can have you write a quick sample 
now—about 300 words on any topic that's comfortable for you.
```

### Step 4: Gather Clarifications
```
Now let me ask a few clarifying questions about your book:
1. What's your book fundamentally about? (1-2 sentence summary)
2. Who is your intended reader? (age, background, what they seek)
3. How many chapters are you envisioning?
4. What should readers gain or learn from it?
```

### Step 5: Document Persona
```
Based on your writing samples and answers, I'm going to create a persona-writing-style.md 
file that documents your voice. Please review it and let me know if it's accurate or 
if I've missed anything about your style.
```

### Step 6: Confirm and Move Forward
```
Great! I've validated everything we need:
✅ Book topic and scope are clear
✅ Your writing voice is documented
✅ Target audience is defined
✅ Resources are accessible

We're ready to move to the Planning phase. Next, we'll outline your book structure 
and plan the writing process chapter by chapter.
```

---

## Key Reminders

- **Don't skip validation**: It seems like extra work, but it prevents confusion and wasted effort later
- **Ask clarifying questions**: If anything is unclear, ask. It's better to clarify now than discover problems mid-writing
- **Document everything**: Persona, scope, assumptions—all go in the framework files
- **Author approval matters**: The author should confirm persona and scope before moving forward
- **Iteration is okay**: If persona or scope changes as you write, update the documentation

---

## Next Steps When Validated

Once this checklist is 100% complete:
→ Proceed to `/framework/process-plan.md` for Phase 1: Planning
