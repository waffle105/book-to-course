# Book To Course Method

This method is inspired by the public concept of "化书成课": turning a book into a shareable, teachable course through deconstruction, integration, reconstruction, extension, innovation, and scenario-based design. Use it as a workflow, not as copied book content.

## Public Source Anchors

The referenced book is:

- Title: `化书成课：培训师快速打造爆款课的秘诀`
- Author: 袁茹锦
- Publisher: 清华大学出版社
- Publication date commonly listed: 2020
- Public summaries describe the method as book-course integration, reading internalization, course development, course positioning, course operation, and scenario-based course design.

Do not claim to know unavailable full text. When the user provides the book file, use that file as the working source.

## Intake Checklist

Capture these facts before designing:

- Book: title, author, edition, language, file type.
- Source depth: full text, table of contents, chapters, notes, or excerpts.
- Target learners: role, level, industry, pain points.
- Course use: public class, internal training, paid course, workshop, bootcamp, or self-study.
- Duration: 30 minutes, 2 hours, half day, 1 day, multi-day, or video course.
- Output: outline only, course package, PPT, workbook, instructor guide, marketing copy.
- Constraints: tone, difficulty, examples, forbidden content, required frameworks.

## Transformation Model

Use six moves:

1. Deconstruct: identify thesis, core concepts, chapter logic, methods, stories, cases, tools, and evidence.
2. Select: keep what serves the course promise; cut material that is interesting but not teachable for the target learner.
3. Reorganize: rebuild around learner problems, tasks, scenarios, and decision points.
4. Translate: turn ideas into frameworks, checklists, worksheets, diagrams, demonstrations, and scripts.
5. Extend: add missing bridges, examples, exercises, cases, and application scenarios.
6. Productize: package the course with positioning, modules, lessons, activities, slides, instructor notes, and learner outputs.

## Deconstruction Template

For each chapter or major section, extract:

- Key question answered by this section.
- Core claim in one sentence.
- Concepts and definitions.
- Method, framework, or process.
- Cases, stories, examples, and data.
- Useful teaching metaphor.
- Application scenario.
- Possible exercise.
- Source anchor: chapter/page/location if available.

## Course Positioning Template

Define:

- Course name.
- One-sentence promise: "After this course, learners can..."
- Target learners.
- Learner pain points.
- Use scenario.
- Prerequisites.
- Course level.
- Duration and delivery mode.
- Final learner output.
- Not included.

## Architecture Patterns

Choose one primary structure:

- Problem-to-solution: pain, cause, method, practice, action plan.
- Capability ladder: awareness, understanding, operation, application, transfer.
- Workflow: prepare, analyze, design, execute, review.
- Case workshop: case setup, diagnosis, tool use, group output, critique.
- Framework-first: model, components, examples, practice, checklist.
- Before-after transformation: old way, new way, method, cases, implementation.

Do not default to the book's chapter order unless the book itself is already a strong teaching sequence.

## Lesson Design Template

For every lesson, specify:

- Lesson title.
- Learner outcome.
- Source ideas used.
- Teaching hook.
- Core concept.
- Visual structure suggestion.
- Demonstration or example.
- Individual exercise.
- Group discussion or peer review.
- Transfer task for learner's real work.
- Instructor notes.
- Time budget.

## Learner Handbook Template

When developing a chapter or lesson in detail, also create a learner-facing handbook or workbook. The handbook is not a slide transcript and not an instructor guide. It should help learners listen, think, fill in, practice, and carry their project to the next lesson.

Recommended structure:

1. Lesson cover and learning map:
   - Course/lesson title.
   - What this lesson solves.
   - What learners will produce.
   - What this lesson feeds into next.
2. Pre-class or opening self-check:
   - What learners already have.
   - What they want to solve.
   - What project or case they will use.
3. Method cards:
   - Core models, formulas, frameworks, comparison tables, or decision rules.
   - Keep each card short enough for classroom use.
4. Case pages:
   - One transformed example.
   - Fields for learner observation, diagnosis, and reusable takeaways.
5. Classroom worksheets:
   - Fill-in tables for the lesson's main practice.
   - Use "我的..." fields so learners produce their own project output.
6. Peer feedback pages:
   - 2-4 prompts or scoring dimensions for pair/group review.
   - Use concrete sentence stems.
7. Self-check page:
   - Criteria for whether the learner's output can move to the next stage.
8. Homework and next-lesson input:
   - Exact deliverable.
   - File/content requirements.
   - What to bring into the next lesson.

Common handbook page types:

- Project brief page.
- Diagnostic checklist.
- Framework mapping table.
- Script or storyboard grid.
- Prompt/template workspace.
- Case analysis worksheet.
- Peer feedback form.
- Quality check rubric.
- After-class action plan.

Avoid:

- Long source-book summaries.
- Instructor timing and facilitation notes.
- Speaker notes.
- Dense theoretical paragraphs.
- Copying large passages from the source book.

## Practice Design Patterns

Use at least one of these in each module:

- Diagnostic checklist.
- Scenario decision.
- Fill-in worksheet.
- Framework mapping.
- Case analysis.
- Role-play.
- Rewrite or redesign task.
- Personal action plan.
- Peer critique.
- Final project.

## Chapter-by-Chapter Output Pattern

When the user asks to develop a book "by chapter" or "one part at a time", create a consistent package for each chapter/lesson:

- `lesson-XX-detailed-teaching-plan.md`: detailed instructor-facing lesson plan.
- `learner-handbooks/lesson-XX-learner-handbook.md` or a clear Chinese filename such as `第X课-学员手册.md`: learner-facing workbook.
- Optional `courseware-output/<lesson-title>/`: visual PPT files when `$generate-courseware` is requested.
- Optional `practice-pack/lesson-XX/`: standalone worksheets, cases, and exercise files when the user asks for a training material package.

For every later chapter, keep section names, worksheet style, checklists, and homework formatting consistent unless the lesson type requires a deliberate change.

## Courseware Handoff

When the user wants PPT, prepare a `courseware-brief.md` with:

- Course title and audience.
- Module structure.
- Slide count target.
- Page role list.
- Visual logic suggestions.
- Style preference.
- Key on-slide text.
- Instructor notes per page.

Then use `$generate-courseware` to create the visual deck. Keep book-to-course responsible for pedagogy and course logic; keep generate-courseware responsible for slide visual production.

## Copyright-Safe Handling

- Quote only short snippets when necessary and only as source anchors.
- Prefer paraphrase and transformation.
- Do not output chapter-length summaries that substitute for the book.
- For paid/public courses, remind the user to check licensing if they want to use extensive original text, diagrams, or proprietary cases.
