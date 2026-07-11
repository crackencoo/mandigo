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
- Current Dashboard, Tasks, and Calendar modules should remain unchanged unless needed for integration

This sprint has two goals:

1. Fix the Quick Capture → Convert to task flow.
2. Build the full Fitness Module.

PART 1 — QUICK CAPTURE CONVERT TO TASK FIX

Current issue:
Quick Capture works and captured items appear inside Recent Captures / Inbox.
However, when the user clicks "Convert to task", the captured item does not get added to Today's Tasks.

Expected behavior:

When the user creates a Quick Capture item and selects type "Task", it should appear in Recent Captures.

When the user clicks "Convert to task":

1. Create a new task from that capture.
2. Add the new task to Today's Tasks on the Dashboard.
3. Add the new task to the Tasks module list.
4. The new task should use:
   - title: captured text
   - category: General
   - status: Not started
   - priority: Medium
   - duration: 15 min
   - description: Created from Quick Capture
5. Show the new task inside Today's Tasks immediately without page refresh.
6. Show a success toast:
   "Capture converted to task"
7. Update the Recent Capture item visually:
   - either mark it as "Converted"
   - or disable the Convert to task button
8. Update dashboard task count and daily completion statistics if needed.
9. The new task should be clickable like other smart task cards.
10. Clicking the new task should open a general task detail view.
11. The general task detail view should include:
   - title
   - category
   - status
   - priority
   - description
   - notes section
   - checklist placeholder
   - Mark as completed button

Also make sure:

- If the capture type is Idea or Note, Convert to task should still work, but it should create a General task.
- The task should also appear in the Tasks page under category General.
- Search and filters in Tasks should include the converted task.
- Completing the converted task should update its status and dashboard progress.

Keep everything in local mock state for now.

PART 2 — FITNESS MODULE v0.1

This sprint also focuses on building the full Fitness Module.

Mandigo is a personal performance operating system. The Fitness module should feel like a premium workout command center, not a basic workout list.

Sprint Goal:
Create a complete Fitness page that allows users to view workouts, open workout details, follow exercise instructions, and complete workouts.

The Fitness page should be accessible from the sidebar when clicking "Fitness".

Fitness Module Requirements:

1. Page Header

Create a polished Fitness page header.

Header content:

Title:
Fitness

Subtitle:
Track your workouts, follow exercise guides, and build consistency.

Add primary action button:
+ New Workout

Add secondary actions:
- Today
- Workout Library
- Exercise Library
- Progress

2. Main Fitness Layout

Create a modern fitness dashboard layout with:

- Today's Workout card
- Weekly workout summary
- Workout library
- Exercise library preview
- Progress statistics
- Recent activity

The layout should feel premium, modular, and connected to the rest of Mandigo.

3. Today's Workout

Create a large featured card:

Title:
Push Day Workout

Workout type:
Hypertrophy

Duration:
65 min

Target muscles:
Chest, shoulders, triceps

Status:
Not started

Show:

- Exercise count: 4 exercises
- Estimated volume
- Completion state
- CTA button: Start Workout

When clicked, open the Workout Detail / Workout Player experience.

4. Workout Library

Create a workout library section with sample workouts:

Workout 1:
Push Day Workout
Type: Hypertrophy
Duration: 65 min
Target: Chest, shoulders, triceps
Status: Not started

Workout 2:
Pull Day Workout
Type: Strength / Hypertrophy
Duration: 70 min
Target: Back, biceps, rear delts
Status: Planned

Workout 3:
Leg Day Workout
Type: Strength
Duration: 75 min
Target: Quads, hamstrings, glutes, calves
Status: Planned

Workout 4:
Mobility Recovery
Type: Recovery
Duration: 25 min
Target: Full body mobility
Status: Optional

Each workout card should show:

- Icon
- Workout name
- Type
- Duration
- Target muscles
- Status
- CTA button: Open / Start

5. Workout Detail / Workout Player

When clicking Push Day Workout or Start Workout, open a polished workout detail screen, modal, drawer, or page.

Workout Detail should show:

- Workout title
- Duration
- Goal
- Target muscles
- Difficulty
- Estimated calories placeholder
- Completion status
- Start / Mark as completed button

Include exercise list:

Exercise 1:
Bench Press
Sets: 4
Reps: 8
Rest: 90 sec
Muscle group: Chest
Instruction:
Keep your shoulder blades retracted, control the eccentric phase, and press explosively without losing tension.
Video placeholder:
Exercise video guide

Exercise 2:
Incline Dumbbell Press
Sets: 3
Reps: 10
Rest: 75 sec
Muscle group: Upper chest
Instruction:
Keep elbows slightly tucked, lower the dumbbells under control, and press through the upper chest.
Video placeholder:
Exercise video guide

Exercise 3:
Shoulder Press
Sets: 3
Reps: 10
Rest: 75 sec
Muscle group: Shoulders
Instruction:
Brace your core, avoid excessive lower back arching, and press overhead with control.
Video placeholder:
Exercise video guide

Exercise 4:
Triceps Pushdown
Sets: 3
Reps: 12
Rest: 60 sec
Muscle group: Triceps
Instruction:
Keep elbows fixed at your sides and fully extend the arms while controlling the return.
Video placeholder:
Exercise video guide

Each exercise card should include:

- Exercise name
- Sets
- Reps
- Rest
- Muscle group badge
- Written instruction
- Video placeholder
- Checkbox or completion toggle

6. Exercise Library

Create an Exercise Library preview section.

Sample exercises:

- Bench Press
- Incline Dumbbell Press
- Shoulder Press
- Triceps Pushdown
- Lat Pulldown
- Squat
- Romanian Deadlift
- Plank

Each exercise item should show:

- Exercise name
- Muscle group
- Equipment
- Difficulty
- Video placeholder icon

Clicking an exercise should open an exercise detail view.

Exercise Detail should show:

- Exercise name
- Muscle group
- Equipment
- Difficulty
- Written instructions
- Common mistakes
- Coaching cues
- Video placeholder

7. Fitness Statistics

Add statistics cards:

- Workouts this week
- Workout consistency
- Total training time
- Completed exercises
- Current streak

Example values:

- Workouts this week: 3 / 5
- Consistency: 80%
- Training time: 210 min
- Completed exercises: 14
- Streak: 4 days

8. Progress Area

Add a progress section showing:

- Weekly training volume
- Workout completion percentage
- Muscle group focus

Use polished progress bars or small chart-like UI elements.

No real chart library is required unless already used in the project.

9. Workout Completion Behavior

When the user clicks "Mark as completed":

- Update workout status to Completed
- Update today's workout card
- Update workout library item
- Update fitness statistics
- Show success toast notification
- If possible, update related Dashboard/Tasks/Calendar state visually

Keep this in local mock state for now.

10. New Workout Modal

When clicking "+ New Workout", open a polished modal.

Fields:

- Workout name
- Workout type
- Duration
- Target muscles
- Difficulty
- Notes

On submit:

- Add new workout to local mock state
- Show success toast
- Display it in the workout library

11. Relationship With Dashboard, Tasks, and Calendar

Fitness should feel connected to existing modules.

- Push Day Workout should match the Dashboard smart task.
- Push Day Workout should match the Tasks module workout task.
- Push Day Workout should match the Calendar fitness event.

Do not break existing Dashboard, Tasks, or Calendar interactions.

If full shared state is too complex, keep visual consistency and mock connection for now.

12. Empty States

Create polished empty states.

Examples:

When no workouts exist:
"No workouts planned"
"Create a workout or choose from the library."

When no exercises match:
"No exercises found"
"Try another muscle group or add a new exercise."

13. Interaction Behavior

Fitness interactions should include:

- Clicking workout opens detail
- Clicking exercise opens detail
- Exercise completion toggles visually
- Workout completion updates state
- New Workout adds workout to local state
- Toast notification after completion or creation
- Smooth transitions

14. Technical Requirements

- Use reusable components
- Keep data mock/local state only
- Do not add authentication
- Do not add database
- Do not connect Supabase yet
- Do not rebuild from scratch
- Maintain responsive design
- Maintain dark/light mode support
- Keep animations subtle and professional

15. Quality Bar

The Fitness page should feel like it belongs in a premium SaaS product.

It should not look like a generic gym tracker.

It should feel like the foundation of a future PT coaching platform.

The final result should make it obvious that Mandigo can evolve into:

- personal workout tracker
- PT client training platform
- exercise education system
- remote coaching dashboard
- admin/member training management system

Build this update now:

- Fix Quick Capture → Convert to task
- Build Sprint 4: Fitness Module v0.1
