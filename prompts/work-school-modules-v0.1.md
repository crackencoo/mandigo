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
- Current Dashboard, Tasks, Calendar, Fitness, and Nutrition modules should remain unchanged unless needed for Work and School integration

This sprint focuses on building two modules in one update:

1. Work Module v0.1
2. School Module v0.1

Mandigo is a personal performance operating system. Work and School should feel like structured daily responsibility modules, not basic note pages.

Sprint Goal:
Create complete Work and School pages that allow users to manage shifts, study blocks, checklists, notes, assignments, resources, deadlines, and completion flows.

The Work page should be accessible from the sidebar when clicking "Work".
The School page should be accessible from the sidebar when clicking "School".

PART 1 — WORK MODULE v0.1

1. Work Page Header

Create a polished Work page header.

Header content:

Title:
Work

Subtitle:
Manage your shifts, work tasks, notes, and daily responsibilities.

Add primary action button:
+ New Shift

Add secondary actions:
- Today
- Schedule
- Notes
- Progress

2. Main Work Layout

Create a modern Work dashboard layout with:

- Today's Shift card
- Work checklist
- Shift schedule
- Work notes
- Work statistics
- Recent work activity

The layout should feel premium, modular, and connected to the rest of Mandigo.

3. Today's Shift Card

Create a large featured card:

Title:
Work Shift

Time:
09:00 - 17:00

Status:
In progress

Location:
Main workplace

Description:
Complete today’s work shift and log notes.

Show:

- Shift duration: 8h
- Checklist progress
- Completion state
- CTA button: Open Shift

When clicked, open the Shift Detail experience.

4. Shift Schedule

Create a shift schedule section with sample shifts:

Shift 1:
Title: Work Shift
Date: Today
Time: 09:00 - 17:00
Status: In progress

Shift 2:
Title: Evening Shift
Date: Tomorrow
Time: 16:00 - 22:00
Status: Planned

Shift 3:
Title: Off Day
Date: Saturday
Time: —
Status: Off

Shift 4:
Title: Short Shift
Date: Sunday
Time: 10:00 - 14:00
Status: Planned

Each shift card should show:

- Shift title
- Date
- Time
- Duration
- Status
- CTA button: Open

5. Shift Detail Experience

When clicking Work Shift or Open Shift, open a polished shift detail screen, modal, drawer, or page.

Shift Detail should show:

- Shift title
- Date
- Time
- Duration
- Location
- Status
- Description
- Checklist
- Notes section
- Mark shift as completed button

Checklist:

- Arrive on time
- Complete main tasks
- Log work notes
- Prepare next shift

Each checklist item should have a completion toggle.

6. Work Notes

Create a Work Notes section.

Sample notes:

Note 1:
Title: Shift reflection
Content: Track what went well and what needs improvement.

Note 2:
Title: Manager feedback
Content: Add important feedback or reminders here.

Note 3:
Title: Next shift preparation
Content: Prepare key items before the next shift.

Each note should show:

- Title
- Short preview
- Timestamp
- CTA: Open

Clicking a note should open a note detail view.

7. Work Statistics

Add work statistics cards:

- Hours this week
- Completed shifts
- Checklist completion
- Focus score
- Next shift

Example values:

- Hours this week: 24h
- Completed shifts: 3
- Checklist completion: 75%
- Focus score: 82%
- Next shift: Tomorrow 16:00

8. Work Completion Behavior

When the user clicks "Mark shift as completed":

- Update shift status to Completed
- Update Today's Shift card
- Update shift schedule item
- Update work statistics
- Show success toast notification
- If possible, update related Dashboard/Tasks/Calendar state visually

Keep this in local mock state for now.

9. New Shift Modal

When clicking "+ New Shift", open a polished modal.

Fields:

- Shift title
- Date
- Start time
- End time
- Location
- Description
- Notes

On submit:

- Add new shift to local mock state
- Show success toast
- Display it in the shift schedule

10. Work Relationship With Dashboard, Tasks, Calendar

Work should feel connected to existing modules.

- Work Shift should match the Dashboard smart task.
- Work Shift should match the Tasks module work task.
- Work Shift should match the Calendar work event.

Do not break existing Dashboard, Tasks, Calendar, Fitness, or Nutrition interactions.

If full shared state is too complex, keep visual consistency and mock connection for now.

PART 2 — SCHOOL MODULE v0.1

1. School Page Header

Create a polished School page header.

Header content:

Title:
School

Subtitle:
Manage your classes, assignments, study blocks, resources, and deadlines.

Add primary action button:
+ New Assignment

Add secondary actions:
- Today
- Classes
- Assignments
- Resources
- Progress

2. Main School Layout

Create a modern School dashboard layout with:

- Today's Study Block card
- Classes section
- Assignments section
- Study checklist
- Resources preview
- School statistics
- Recent school activity

The layout should feel premium, modular, and connected to the rest of Mandigo.

3. Today's Study Block Card

Create a large featured card:

Title:
School Review

Duration:
45 min

Status:
Not started

Focus:
Digital Marketing notes review

Description:
Review lecture notes and complete the study checklist.

Show:

- Duration
- Checklist progress
- Completion state
- CTA button: Start Review

When clicked, open the Study Detail experience.

4. Classes Section

Create a classes section with sample classes:

Class 1:
Title: Digital Marketing Strategy
Time: Monday 10:00
Status: Active

Class 2:
Title: Consumer Behavior
Time: Wednesday 12:00
Status: Active

Class 3:
Title: Analytics and Reporting
Time: Friday 09:00
Status: Active

Each class card should show:

- Class title
- Time
- Status
- Next session
- CTA button: Open

5. Assignments Section

Create an assignments section with sample assignments:

Assignment 1:
Title: Campaign Analysis Report
Class: Digital Marketing Strategy
Due date: Friday
Status: In progress
Priority: High

Assignment 2:
Title: Consumer Persona Task
Class: Consumer Behavior
Due date: Next Monday
Status: Not started
Priority: Medium

Assignment 3:
Title: Analytics Dashboard Review
Class: Analytics and Reporting
Due date: Wednesday
Status: Planned
Priority: Medium

Each assignment card should show:

- Assignment title
- Class
- Due date
- Status
- Priority
- CTA button: Open

6. Study Detail Experience

When clicking School Review or Start Review, open a polished study detail screen, modal, drawer, or page.

Study Detail should show:

- Title
- Duration
- Focus
- Status
- Description
- Study checklist
- Resources
- Notes section
- Mark study block as completed button

Study checklist:

- Review lecture notes
- Summarize key concepts
- Complete assignment checklist
- Write questions for next class

Each checklist item should have a completion toggle.

Resources:

- Lecture notes
- Assignment checklist
- Review questions
- Presentation slides placeholder

7. Assignment Detail Experience

When clicking an assignment, open assignment detail.

Assignment Detail should show:

- Assignment title
- Class
- Due date
- Status
- Priority
- Description
- Checklist
- Resources
- Notes
- Mark as completed button

Checklist example:

- Read assignment brief
- Collect resources
- Draft outline
- Complete final version
- Submit assignment

8. Resources Section

Create a Resources preview section.

Sample resources:

- Digital Marketing lecture notes
- Campaign analysis template
- Consumer persona worksheet
- Analytics reporting checklist
- Presentation slides placeholder

Each resource should show:

- Resource title
- Type
- Related class
- CTA: Open

Clicking resource opens resource detail view.

9. School Statistics

Add school statistics cards:

- Study time this week
- Assignments completed
- Upcoming deadlines
- Study consistency
- Current focus

Example values:

- Study time this week: 6h
- Assignments completed: 2
- Upcoming deadlines: 3
- Study consistency: 78%
- Current focus: Digital Marketing

10. School Completion Behavior

When the user clicks "Mark study block as completed":

- Update study block status to Completed
- Update Today's Study Block card
- Update school statistics
- Show success toast notification
- If possible, update related Dashboard/Tasks/Calendar state visually

When the user clicks "Mark assignment as completed":

- Update assignment status to Completed
- Update assignments section
- Update school statistics
- Show success toast notification

Keep this in local mock state for now.

11. New Assignment Modal

When clicking "+ New Assignment", open a polished modal.

Fields:

- Assignment title
- Class
- Due date
- Status
- Priority
- Description
- Notes

On submit:

- Add new assignment to local mock state
- Show success toast
- Display it in the assignments section

12. School Relationship With Dashboard, Tasks, Calendar

School should feel connected to existing modules.

- School Review should match the Dashboard smart task.
- School Review should match the Tasks module school task.
- School Review Block should match the Calendar school event.

Do not break existing Dashboard, Tasks, Calendar, Fitness, Nutrition, or Work interactions.

If full shared state is too complex, keep visual consistency and mock connection for now.

SHARED REQUIREMENTS FOR WORK AND SCHOOL

1. Empty States

Create polished empty states for both modules.

Work examples:

- No shifts scheduled
- No work notes yet
- No checklist items

School examples:

- No assignments
- No classes
- No resources

2. Interaction Behavior

Work interactions should include:

- Clicking shift opens detail
- Clicking note opens note detail
- Checklist toggles visually
- Mark shift as completed updates state
- New Shift adds shift to local state
- Toast notification after shift completion or creation

School interactions should include:

- Clicking study block opens detail
- Clicking class opens detail
- Clicking assignment opens detail
- Clicking resource opens detail
- Checklist toggles visually
- Mark study block as completed updates state
- Mark assignment as completed updates state
- New Assignment adds assignment to local state
- Toast notification after completion or creation

3. Technical Requirements

- Use reusable components
- Keep data mock/local state only
- Do not add authentication
- Do not add database
- Do not connect Supabase yet
- Do not rebuild from scratch
- Maintain responsive design
- Maintain dark/light mode support
- Keep animations subtle and professional

4. Quality Bar

Work and School pages should feel like they belong in a premium SaaS product.

They should not look like basic note pages.

They should feel like the foundation of a future personal performance system and admin/member productivity platform.

The final result should make it obvious that Mandigo can evolve into:

- personal life management system
- student productivity platform
- work routine tracker
- PT client lifestyle tracking system
- admin/member performance dashboard

Build this update now:

- Sprint 6: Work Module v0.1
- Sprint 7: School Module v0.1
