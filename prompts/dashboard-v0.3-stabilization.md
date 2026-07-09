Continue improving the existing Mandigo Dashboard v0.2.

Do not redesign the app. Keep the current layout, sidebar, visual style, dark mode, cards, purple/blue accent colors, and smart task widget design.

This is a stabilization update.

Fix Quick Capture:

Currently, Quick Capture opens a modal, but submitted content does not appear anywhere.

Expected behavior:

When the user submits a Quick Capture item, it should be saved in local mock state and displayed immediately in a new dashboard widget called "Recent Captures" or "Inbox".

Add a new widget under or near Quick Actions:

Widget title:
Recent Captures

Each captured item should show:
- content text
- type badge: Idea / Task / Note
- timestamp such as "Just now"
- small action button: Convert to task

Quick Capture modal should include:
- text input
- type selector: Idea, Task, Note
- submit button
- cancel button

After submit:
- close modal
- show the new item in Recent Captures
- show a subtle success feedback

Also improve task completion interactions:

When the user clicks "Mark as completed" inside a task detail view:
- update the task status to Completed
- update the task card on the dashboard
- update daily completion percentage
- update progress/statistics visually
- close the detail modal or show a completed state

Keep all data as mock local state for now.

Do not add authentication.
Do not add a database.
Do not connect Supabase.
Do not rebuild the whole app.

Focus only on:
- Quick Capture persistence in mock state
- Recent Captures widget
- task completion state updates
- dashboard progress updates
