Continue building the existing Mandigo application.

Do not rebuild the whole app from scratch.

Keep the current approved Mandigo design direction:

- Premium dark SaaS interface
- Light/dark mode support
- Left sidebar navigation
- Purple and blue accent colors
- Rounded cards
- Smooth interactions
- Minimal, clean, professional layout
- Current Dashboard design should remain mostly unchanged

This sprint focuses on building the full Tasks Module.

Mandigo is not a simple todo app.

In Mandigo, a task can be a smart interactive module. A task can open a detailed experience with instructions, media placeholders, progress, checklists, and completion feedback.

Sprint Goal:
Create a complete Tasks page that acts as the central task management system behind the Dashboard smart task widgets.

The Tasks page should be accessible from the sidebar when clicking "Tasks".

Tasks Module Requirements:

1. Page Header

Create a polished Tasks page header.

Header content:

Title:
Tasks

Subtitle:
Manage your daily modules, routines, and responsibilities.

Add a primary action button:
+ New Task

Add secondary actions:
- Filter
- Sort
- View options

2. Main Tasks Layout

Create a modern task management layout with:

- Today section
- Upcoming section
- Completed section
- Category filters
- Status filters
- Search input

The layout should feel like a premium productivity tool, not a basic todo list.

3. Task Categories

Support these task categories:

- General
- Fitness
- Nutrition
- Work
- School

Each category should have:

- Icon
- Color accent
- Badge style

4. Task Statuses

Support these statuses:

- Not started
- In progress
- Completed
- Waiting
- Skipped

Statuses should be visually clear.

5. Task Priority

Support priority levels:

- Low
- Medium
- High

Display priority as small badges or indicators.

6. Task List Items

Each task item should show:

- Task title
- Category badge
- Status badge
- Priority
- Time or duration
- Short description
- CTA button

CTA examples:

- Open
- Start
- Review
- Continue

Task items should feel clickable.

7. Sample Tasks

Use these mock tasks:

Task 1:
Title: Work Shift
Category: Work
Time: 09:00 - 17:00
Status: In progress
Priority: High
Description: Complete today’s work shift and log notes.

Task 2:
Title: Push Day Workout
Category: Fitness
Duration: 65 min
Status: Not started
Priority: High
Description: Chest, shoulders, and triceps workout.

Task 3:
Title: Meal Prep
Category: Nutrition
Duration: 30 min
Status: Not started
Priority: Medium
Description: Prepare meals according to today’s macro target.

Task 4:
Title: School Review
Category: School
Duration: 45 min
Status: Not started
Priority: Medium
Description: Review lecture notes and complete study checklist.

Task 5:
Title: Quick Planning
Category: General
Duration: 15 min
Status: Waiting
Priority: Low
Description: Organize today’s priorities and capture ideas.

8. Task Detail Experience

When clicking any task, open a detail screen, modal, drawer, or dedicated page.

The detail experience should depend on task type.

General Task Detail:
- Title
- Category
- Status
- Priority
- Description
- Notes section
- Checklist
- Mark as completed button

Workout Task Detail:
Title: Push Day Workout
Duration: 65 min

Show workout summary:

- Goal: Hypertrophy
- Target muscles: Chest, shoulders, triceps
- Estimated duration: 65 min

Exercises:

1. Bench Press
- 4 sets x 8 reps
- 90 sec rest
- Written instruction placeholder
- Video guide placeholder

2. Incline Dumbbell Press
- 3 sets x 10 reps
- 75 sec rest
- Written instruction placeholder
- Video guide placeholder

3. Shoulder Press
- 3 sets x 10 reps
- 75 sec rest
- Written instruction placeholder
- Video guide placeholder

4. Triceps Pushdown
- 3 sets x 12 reps
- 60 sec rest
- Written instruction placeholder
- Video guide placeholder

Add:
- Exercise video guide card
- Written instructions section
- Mark as completed button

Meal Prep Task Detail:
Title: Meal Prep
Duration: 30 min

Show nutrition summary:

- Calories: 2800 kcal
- Protein: 180g
- Carbs: 300g
- Fats: 75g

Meals:

1. Chicken rice bowl
2. Greek yogurt protein snack
3. Egg and avocado toast

Add:
- Recipe section
- Preparation steps
- Video/recipe placeholder
- Mark as completed button

Work Task Detail:
Title: Work Shift
Time: 09:00 - 17:00

Show:

- Shift time
- Work checklist
- Notes section

Checklist:
- Arrive on time
- Complete main tasks
- Log work notes

Add:
- Mark as completed button

School Task Detail:
Title: School Review
Duration: 45 min

Show:

- Study goal
- Resources
- Assignment checklist

Resources:
- Lecture notes
- Assignment checklist
- Review questions

Add:
- Mark as completed button

9. Completion Behavior

When clicking "Mark as completed":

- Update the task status to Completed
- Show a success toast notification
- Update task card/list item visually
- Update completion statistics
- Keep data in local mock state for now

10. Task Statistics

Add a small statistics area on the Tasks page.

Show:

- Total tasks
- Completed today
- In progress
- Completion percentage
- High priority tasks

11. Filters

Add functional mock filters:

Filter by category:

- All
- General
- Fitness
- Nutrition
- Work
- School

Filter by status:

- All
- Not started
- In progress
- Completed
- Waiting
- Skipped

When a filter is clicked, visually update the selected filter state and filter the displayed mock tasks.

12. Empty States

Create polished empty states.

Examples:

When no tasks match a filter:
"No tasks found"
"Try changing your filters or create a new task."

When all tasks are completed:
"All clear"
"Your day is complete."

13. New Task Modal

When clicking "+ New Task", open a polished modal.

Fields:

- Task title
- Category
- Status
- Priority
- Time or duration
- Description
- Task type

Task types:

- General
- Workout
- Meal Prep
- Work
- School

On submit:

- Add the new task to local mock state
- Show success toast
- Display it in the task list

14. Relationship With Dashboard

Keep Dashboard and Tasks visually consistent.

The Tasks module should feel like the deeper system behind the Dashboard smart widgets.

Do not break existing Dashboard interactions.

15. Technical Requirements

- Use reusable components
- Keep data mock/local state only
- Do not add authentication
- Do not add database
- Do not connect Supabase yet
- Do not rebuild from scratch
- Maintain responsive design
- Maintain dark/light mode support
- Keep animations subtle and professional

16. Quality Bar

The Tasks page should feel like it belongs in a premium SaaS product.

It should not look like a basic checklist app.

It should feel modular, interactive, and ready to evolve into:

- personal productivity system
- fitness tracking system
- PT client management system
- admin/member platform

Build Sprint 2: Tasks Module now.
