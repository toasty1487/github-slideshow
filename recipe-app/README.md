# 🍳 Macro Kitchen — Recipe Finder

A tiny, self-contained recipe app with **150 fresh, wholesome recipes** balanced
across every macro × diet category. Pick a **macro focus** and a **diet**, and it
shows matching meals with ingredients, method, and per-serving nutrition.

## Features

- **Favourites:** tap the ♡ on any recipe to save it, then use the **❤️ Favourites** toggle to see just your saved recipes. Kept in `localStorage`.

- **Three languages with a selector:** English, Dutch (Nederlands), and German
  (Deutsch). The EN/NL/DE switch in the top-right translates the whole interface
  *and* every recipe — names, ingredients, and steps — and your choice is
  remembered between visits. Goal descriptions are understood in all three
  languages too.
- **Describe your goal in plain English:** type something like *"build muscle,
  high protein vegetarian, quick"* or *"lose weight, light and quick"* and the app
  interprets it — setting the macro/diet filters and re-ranking every meal by how
  well it fits, with a short "why this meal" line on each card
- **Macro focus:** More protein 💪 · More fat 🥑 · More carbs 🍚
- **Diet:** Vegan 🌱 · Vegetarian 🧀 · Meat 🍗 (vegan recipes also show under vegetarian)
- Filters combine — every macro × diet combination has at least one recipe
- Protein / fat / carb bars and calories per serving on every card
- Expandable ingredients + step-by-step method
- **Grocery list:** add any recipes to a shopping list — ingredients are combined
  across recipes (shared items show a `×N` count), tick items off as you shop,
  and copy the whole list to your clipboard
- **Saved between visits:** your grocery list, ticked items, and pantry selection
  are stored in `localStorage`, so they're still there next time you open the app
- **Cook from what you have:** the "What can I make?" panel lets you tick the
  ingredients in your kitchen and instantly see which meals you can make right now
  (and which are one or two items short), then build the meal or add missing items
  to your grocery list
- **Guided step-by-step cooking:** hit "Cook step-by-step" on any meal for a
  full-screen guided plan — mise en place first, then one step at a time with a
  progress bar and Back/Next controls, ending in a "meal is ready" screen
- **Scale by servings:** a −/+ stepper on each recipe rescales every ingredient
  quantity (with tidy fractions like `1½`), and the new amounts flow through to
  the guided plan and the grocery list
- **Weekly plan builder:** compose a whole week in one tap — **breakfast, lunch,
  dinner and a light snack per day** — to your **kcal/day, protein/day and
  max-carbs/day** targets, with per-day badges showing how each day measures up.
  Portions of the three main meals **scale automatically to hit your calorie
  target** (the snack stays a fixed fruit + nuts sized extra). Keep the same
  breakfast all week (with subtle daily toppings), swap any single meal, and get
  a **combined shopping list grouped by aisle** (produce, meat & fish, dairy,
  bread, pantry) with quantities summed across the week. Ships with 23 breakfasts
  and 14 snacks across all diets.
- No build step, no dependencies, works offline

## Run it

Just open `index.html` in any browser — that's it.

To serve it locally instead:

```bash
cd recipe-app
python3 -m http.server 8000   # then visit http://localhost:8000
```

> Nutrition values are approximate, per serving.
