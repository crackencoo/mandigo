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
- Current Dashboard, Tasks, Calendar, and Fitness modules should remain unchanged unless needed for Nutrition integration

This sprint focuses on building the full Nutrition Module.

Mandigo is a personal performance operating system. The Nutrition module should feel like a premium meal prep and nutrition command center, not a basic calorie tracker.

Sprint Goal:
Create a complete Nutrition page that allows users to view daily nutrition targets, follow meal prep instructions, open meal details, track macros, and complete nutrition tasks.

The Nutrition page should be accessible from the sidebar when clicking "Nutrition".

Nutrition Module Requirements:

1. Page Header

Create a polished Nutrition page header.

Header content:

Title:
Nutrition

Subtitle:
Track your meals, macros, hydration, and meal prep consistency.

Add primary action button:
+ New Meal

Add secondary actions:
- Today
- Meal Plan
- Recipes
- Progress

2. Main Nutrition Layout

Create a modern nutrition dashboard layout with:

- Today’s Nutrition Summary
- Daily macro targets
- Meal Prep task card
- Today’s meals
- Hydration tracker
- Recipe library preview
- Nutrition statistics
- Recent activity

The layout should feel premium, modular, and connected to the rest of Mandigo.

3. Today’s Nutrition Summary

Create a large featured card:

Title:
Today’s Nutrition

Daily target:
2800 kcal

Macros:
- Protein: 180g
- Carbs: 300g
- Fats: 75g

Hydration:
3L target

Status:
In progress

Show:

- Calories consumed
- Calories remaining
- Protein progress
- Carb progress
- Fat progress
- Water progress
- CTA button: Open Meal Plan

Use polished progress bars or circular progress-style UI elements.

4. Meal Prep Task

Create a smart Meal Prep card:

Title:
Meal Prep

Duration:
30 min

Category:
Nutrition

Status:
Not started

Description:
Prepare meals according to today’s macro target.

CTA:
Open

When clicked, open the Meal Prep Detail experience.

5. Today’s Meals

Create a meals section with sample meals:

Meal 1:
Chicken Rice Bowl
Calories: 850 kcal
Protein: 55g
Carbs: 90g
Fats: 22g
Status: Planned

Meal 2:
Greek Yogurt Protein Snack
Calories: 420 kcal
Protein: 45g
Carbs: 35g
Fats: 10g
Status: Planned

Meal 3:
Egg and Avocado Toast
Calories: 650 kcal
Protein: 35g
Carbs: 55g
Fats: 30g
Status: Planned

Meal 4:
Protein Shake
Calories: 300 kcal
Protein: 35g
Carbs: 20g
Fats: 5g
Status: Optional

Each meal card should show:

- Meal name
- Calories
- Protein
- Carbs
- Fats
- Status
- CTA button: Open / Log

6. Meal Detail Experience

When clicking a meal, open a polished meal detail screen, modal, drawer, or page.

Meal Detail should show:

- Meal title
- Calories
- Protein
- Carbs
- Fats
- Meal type
- Preparation time
- Ingredients
- Preparation steps
- Recipe notes
- Video/recipe placeholder
- Mark as eaten button

Example for Chicken Rice Bowl:

Title:
Chicken Rice Bowl

Calories:
850 kcal

Macros:
Protein: 55g
Carbs: 90g
Fats: 22g

Ingredients:
- Chicken breast
- Rice
- Olive oil
- Mixed vegetables
- Spices

Preparation steps:
1. Cook rice.
2. Season and cook chicken.
3. Prepare vegetables.
4. Combine ingredients in a bowl.
5. Add sauce or spices if needed.

Video placeholder:
Meal prep video guide

Button:
Mark as eaten

7. Meal Prep Detail

When clicking Meal Prep, open a Meal Prep Detail experience.

Meal Prep Detail should show:

- Title: Meal Prep
- Duration: 30 min
- Daily calorie target
- Macro targets
- Meals to prepare
- Shopping list
- Preparation steps
- Recipe/video placeholder
- Completion button

Meals to prepare:

- Chicken rice bowl
- Greek yogurt protein snack
- Egg and avocado toast

Shopping list:

- Chicken breast
- Rice
- Eggs
- Avocado
- Greek yogurt
- Vegetables
- Olive oil

Preparation steps:

1. Prepare ingredients.
2. Cook main protein source.
3. Cook carb source.
4. Assemble meals.
5. Store meals properly.

Button:
Mark meal prep as completed

8. Hydration Tracker

Add hydration tracking section.

Target:
3L water

Show:

- Current intake
- Remaining amount
- Quick buttons:
  - +250ml
  - +500ml
  - +1L

When clicking water buttons:

- Update water intake in local mock state
- Update hydration progress visually
- Show subtle feedback

9. Recipe Library Preview

Create a Recipe Library preview section.

Sample recipes:

- Chicken Rice Bowl
- Egg and Avocado Toast
- Greek Yogurt Protein Snack
- Tuna Pasta Bowl
- Oat Protein Breakfast
- Turkey Wrap

Each recipe item should show:

- Recipe name
- Calories
- Protein
- Prep time
- Difficulty
- CTA: Open

Clicking a recipe should open a recipe detail view.

Recipe Detail should show:

- Recipe name
- Calories
- Macros
- Ingredients
- Preparation steps
- Notes
- Video placeholder

10. Nutrition Statistics

Add nutrition statistics cards:

- Calories today
- Protein progress
- Nutrition adherence
- Meal prep streak
- Water intake

Example values:

- Calories today: 2220 / 2800 kcal
- Protein: 135 / 180g
- Nutrition adherence: 88%
- Meal prep streak: 4 days
- Water intake: 2.0 / 3.0L

11. Progress Area

Add a progress section showing:

- Weekly nutrition adherence
- Average protein intake
- Meal prep completion
- Hydration consistency

Use polished progress bars or small chart-like UI elements.

No real chart library is required unless already used in the project.

12. Nutrition Completion Behavior

When the user clicks "Mark as eaten":

- Update meal status to Eaten
- Update calories consumed
- Update macro progress
- Update nutrition statistics
- Show success toast notification

When the user clicks "Mark meal prep as completed":

- Update Meal Prep task status to Completed
- Update nutrition statistics
- Show success toast notification
- If possible, update related Dashboard/Tasks/Calendar state visually

Keep this in local mock state for now.

13. New Meal Modal

When clicking "+ New Meal", open a polished modal.

Fields:

- Meal name
- Meal type
- Calories
- Protein
- Carbs
- Fats
- Preparation time
- Ingredients
- Notes

On submit:

- Add new meal to local mock state
- Show success toast
- Display it in Today’s Meals or Recipe Library

14. Relationship With Dashboard, Tasks, Calendar, and Fitness

Nutrition should feel connected to existing modules.

- Meal Prep should match the Dashboard smart task.
- Meal Prep should match the Tasks module nutrition task.
- Meal Prep Window should match the Calendar nutrition event.
- Nutrition should complement Fitness for performance tracking.

Do not break existing Dashboard, Tasks, Calendar, or Fitness interactions.

If full shared state is too complex, keep visual consistency and mock connection for now.

15. Empty States

Create polished empty states.

Examples:

When no meals exist:
"No meals planned"
"Create a meal or choose from the recipe library."

When no recipes match:
"No recipes found"
"Try another search or add a new recipe."

When hydration is complete:
"Hydration goal reached"
"Great job staying consistent."

16. Interaction Behavior

Nutrition interactions should include:

- Clicking meal opens meal detail
- Clicking recipe opens recipe detail
- Clicking Meal Prep opens meal prep detail
- Mark as eaten updates meal state
- Meal prep completion updates state
- Hydration buttons update progress
- New Meal adds meal to local state
- Toast notification after meal logging, meal prep completion, water update, or meal creation
- Smooth transitions

17. Technical Requirements

- Use reusable components
- Keep data mock/local state only
- Do not add authentication
- Do not add database
- Do not connect Supabase yet
- Do not rebuild from scratch
- Maintain responsive design
- Maintain dark/light mode support
- Keep animations subtle and professional

18. Quality Bar

The Nutrition page should feel like it belongs in a premium SaaS product.

It should not look like a generic calorie tracker.

It should feel like the foundation of a future PT coaching and nutrition support platform.

The final result should make it obvious that Mandigo can evolve into:

- personal nutrition tracker
- meal prep planner
- PT client nutrition dashboard
- remote coaching nutrition system
- admin/member nutrition management platform

Build Sprint 5: Nutrition Module v0.1 now.
