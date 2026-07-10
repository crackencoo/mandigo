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
- Current Dashboard and Tasks module should remain unchanged unless needed for Calendar integration

This sprint focuses on building the full Calendar Module.

Mandigo is not just a task manager.

Mandigo is a personal performance operating system where tasks, events, workouts, meal prep, school blocks, and work shifts are connected inside one daily planning system.

Sprint Goal:
Create a full Calendar page that acts as the time-based planning system behind the Dashboard and Tasks modules.

The Calendar page should be accessible from the sidebar when clicking "Calendar".

Calendar Module Requirements:

1. Page Header

Create a polished Calendar page header.

Header content:

Title:
Calendar

Subtitle:
Plan your work, training, meals, school, and personal events in one place.

Add primary action button:
+ New Event

Add secondary actions:
- Today
- Day view
- Week view
- Month view

2. Main Calendar Layout

Create a modern calendar layout with:

- Left side: calendar timeline
- Right side: event details / daily summary panel

The layout should feel like a premium productivity calendar, not a basic date picker.

Default view:
Week view

Also include tabs or buttons for:

- Day
- Week
- Month

3. Calendar Event Types

Support these event types:

- Work
- Fitness
- Nutrition
- School
- Personal
- General

Each event type should have:

- Icon
- Accent color
- Badge style

4. Sample Events

Use these mock events:

Event 1:
Title: Work Shift
Type: Work
Time: 09:00 - 17:00
Description: Main work shift for the day.
Linked task: Work Shift

Event 2:
Title: Meal Prep Window
Type: Nutrition
Time: 12:30 - 13:00
Description: Prepare meals according to today’s macro target.
Linked task: Meal Prep

Event 3:
Title: Push Day Workout
Type: Fitness
Time: 17:30 - 18:45
Description: Chest, shoulders, and triceps workout.
Linked task: Push Day Workout

Event 4:
Title: School Review Block
Type: School
Time: 20:00 - 20:45
Description: Review lecture notes and complete school checklist.
Linked task: School Review

Event 5:
Title: Quick Planning
Type: General
Time: 21:00 - 21:15
Description: Organize tomorrow’s priorities and capture ideas.
Linked task: Quick Planning

5. Week View

Create a clean week view.

Requirements:

- Show days of the week horizontally
- Show time blocks vertically
- Display events as colored blocks
- Events should show:
  - title
  - time
  - type badge or icon
- Current day should be visually highlighted
- Clicking an event should open its detail view

6. Day View

Create a day view.

Requirements:

- Show selected day timeline
- Events stacked by time
- Show daily summary at the top:
  - total events
  - work hours
  - workout planned
  - meal prep planned
  - school block planned

7. Month View

Create a month grid.

Requirements:

- Show event dots or small labels inside dates
- Current day highlighted
- Clicking a day should update selected day panel
- Keep the design clean and not overcrowded

8. Event Detail Experience

When clicking any event, open a modal, drawer, or detail panel.

Event detail should show:

- Event title
- Event type
- Time
- Duration
- Description
- Linked task
- Notes section
- CTA button

CTA button behavior:

If event has linked task:
Button text:
Open Linked Task

Clicking it should open the related task detail experience if possible.

If not possible yet, show a placeholder task detail panel.

9. New Event Modal

When clicking "+ New Event", open a polished modal.

Fields:

- Event title
- Event type
- Date
- Start time
- End time
- Description
- Linked task optional
- Notes

On submit:

- Add the new event to local mock state
- Show success toast
- Display it in the calendar
- Update daily summary

10. Calendar and Tasks Relationship

Calendar events should feel connected to tasks.

Examples:

- Push Day Workout calendar event links to Push Day Workout task
- Meal Prep Window links to Meal Prep task
- Work Shift links to Work Shift task
- School Review Block links to School Review task

Do not break the existing Tasks module.

If a linked task is completed in Tasks, the Calendar event can visually show a subtle completed state.

If this is too complex, keep it as mock visual state for now.

11. Calendar Statistics

Add a small statistics area or right panel showing:

- Events today
- Work hours today
- Training time today
- Nutrition blocks today
- Study time today

Example:

Today’s Schedule Summary:

- 5 events
- 8h work
- 75 min training
- 30 min meal prep
- 45 min study

12. Empty States

Create polished empty states.

Examples:

When a day has no events:
"No events scheduled"
"Add a new event or drag a task into your calendar."

When month has no events:
"Your month is clear"
"Start by planning your work, workouts, meals, or school blocks."

13. Interaction Behavior

Calendar interactions should include:

- Clicking an event opens detail
- Clicking a day selects that day
- Changing view updates calendar layout
- New Event adds event to local state
- Toast notification after event creation
- Smooth transitions between views

14. Quick Actions

Add quick action buttons inside Calendar:

- Add Work Shift
- Add Workout
- Add Meal Prep
- Add School Block
- Add Personal Event

These can open the New Event modal with preselected event type.

15. Relationship With Dashboard

Keep Dashboard and Calendar visually consistent.

The Calendar module should feel like the deeper system behind the Dashboard "Today's Calendar" widget.

Do not break existing Dashboard interactions.

16. Technical Requirements

- Use reusable components
- Keep data mock/local state only
- Do not add authentication
- Do not add database
- Do not connect Supabase yet
- Do not rebuild from scratch
- Maintain responsive design
- Maintain dark/light mode support
- Keep animations subtle and professional

17. Quality Bar

The Calendar page should feel like it belongs in a premium SaaS product.

It should not look like a basic calendar.

It should feel modular, interactive, and ready to evolve into:

- personal planning system
- fitness schedule system
- PT client scheduling system
- work/school productivity planner
- admin/member scheduling platform

Build Sprint 3: Calendar Module now.
