---
name: book-to-course
description: Transform a book, manuscript, reading notes, PDF, DOCX, ebook excerpt, or book outline into a teachable course. Use when Codex needs to turn book content into course positioning, learner outcomes, module structure, detailed lesson plans, learner handbooks/workbooks, practice activities, case discussions, instructor notes, and downstream visual courseware prompts; especially for Chinese "化书成课" workflows.
---

# Book To Course

## Core Rule

Do not make a book summary. Develop a course product.

Turn the source book into a teachable system with audience, problems, learning outcomes, modules, lessons, learner handbooks, practice worksheets, cases, instructor guidance, and optional handoff to `$generate-courseware` for visual PPT production.

Respect copyright:

- Use user-provided book files or excerpts as source material for transformation.
- Do not reproduce long passages from the book.
- Paraphrase, restructure, synthesize, and cite chapter/page anchors when available.
- If the user has not provided the book text, work only from public metadata and ask for the file before detailed course development.

## Workflow

Read `references/book-to-course-method.md` before developing a course.

Use this sequence:

1. Source intake: identify the book title, author, format, audience, page/chapter structure, and available source depth.
2. Course positioning: define target learners, real-world problem, course promise, use scenario, and deliverable format.
3. Book deconstruction: extract the book's core thesis, major knowledge blocks, concepts, methods, cases, tools, and examples.
4. Teaching reconstruction: reorganize book knowledge around learner problems, not the book's original chapter order.
5. Course architecture: create modules, lessons, outcomes, practice tasks, cases, and assessment checkpoints.
6. Lesson design: for every lesson, define input, concept, demonstration, exercise, discussion, reflection, and transfer task.
7. Learner handbook: for every chapter/lesson developed in detail, create a learner-facing workbook with method cards, examples, fill-in worksheets, project pages, checklists, peer feedback forms, and homework.
8. Courseware handoff: if slides are requested, produce a page-level courseware plan and invoke `$generate-courseware` for visual slide generation.
9. Instructor package: provide speaker notes, facilitation tips, timing, learner prompts, and likely misconceptions.

## Required Outputs

For a normal request, create:

- `course-positioning.md`: audience, pain points, course promise, level, duration, and delivery mode.
- `book-deconstruction.md`: thesis, knowledge map, method list, case/example list, reusable quotes only as short anchors, and source locations when known.
- `course-outline.md`: module and lesson structure with learning outcomes.
- `lesson-design.md`: detailed design for each lesson.
- `practice-and-assessment.md`: exercises, worksheets, discussion prompts, assignments, and evaluation criteria.
- `learner-handbook.md` or `learner-handbooks/<lesson-name>.md`: learner-facing workbook pages with method cards, classroom worksheets, project templates, checks, peer feedback, and homework. For chapter-by-chapter course development, create one handbook per lesson/chapter.
- `courseware-brief.md`: page-level plan for a visual PPT if the user wants slides.
- `instructor-guide.md`: teaching flow, timing, notes, transitions, and facilitation suggestions.

Use a compact output when the user only asks for a quick plan.

## Course Design Standards

Make the course useful for adults:

- Start from learner tasks and problems.
- Convert abstract concepts into tools, frameworks, decisions, checklists, and practice.
- Keep each lesson focused on one capability.
- Include cases and scenarios, not only theory.
- Add exercises that make learners apply the book's ideas to their own work.
- Add learner handbook pages that support in-class completion, note-taking, project progress, self-checking, and after-class transfer.
- Make the final deliverable explicit: action plan, worksheet, checklist, case solution, prompt pack, or project output.

## Learner Handbook Standards

Do not make the learner handbook a copy of the lesson plan or slide script. Make it a classroom workbook for learners.

For each detailed lesson/chapter, include:

- Learning map: what this lesson solves, what learners will produce, and how it connects to the next lesson.
- Method cards: concise frameworks, formulas, checklists, or comparison tables learners can reuse.
- Case pages: short transformed examples with fields for learner observations.
- Fill-in worksheets: project brief, diagnosis table, script grid, storyboard table, checklist, or other task-specific pages.
- Peer feedback pages: simple sentence stems or scoring grids for classroom exchange.
- Self-check pages: criteria that help learners judge whether their output can move to the next lesson.
- Homework page: exact after-class deliverable and required inputs for the next lesson.

Keep handbook language learner-facing:

- Use "我/我的" fields and blank spaces for completion.
- Avoid instructor-only timing, speaker notes, and facilitation advice.
- Avoid long book summaries and long quoted passages.
- Keep concepts concise; leave deep explanation to the instructor guide and slides.

When generating PPT, coordinate with `$generate-courseware`:

- Use this skill for course logic and teaching design.
- Use `$generate-courseware` for visual slide style, image-page generation, and PowerPoint assembly.
- Pass course positioning, module structure, lesson objectives, visual logic suggestions, and instructor notes into the courseware skill.

## Quality Gate

Before finalizing, check:

- The course is not a chapter-by-chapter book report.
- Every module maps to a learner problem or capability.
- Every lesson has an outcome and an activity.
- Every detailed chapter/lesson has a learner handbook or workbook section that learners can fill in.
- Abstract ideas have been turned into visual structures, tools, or exercises.
- The course can be delivered by an instructor without rereading the source book during class.
- Copyright-sensitive text is minimized and transformed.
