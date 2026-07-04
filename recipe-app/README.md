# 🍳 Macro Kitchen — Recipe Finder

A tiny, self-contained recipe app. Pick a **macro focus** and a **diet**, and it
shows matching meals with ingredients, method, and per-serving nutrition.

## Features

- **Macro focus:** More protein 💪 · More fat 🥑 · More carbs 🍚
- **Diet:** Vegan 🌱 · Vegetarian 🧀 · Meat 🍗 (vegan recipes also show under vegetarian)
- Filters combine — every macro × diet combination has at least one recipe
- Protein / fat / carb bars and calories per serving on every card
- Expandable ingredients + step-by-step method
- **Grocery list:** add any recipes to a shopping list — ingredients are combined
  across recipes (shared items show a `×N` count), tick items off as you shop,
  and copy the whole list to your clipboard
- No build step, no dependencies, works offline

## Run it

Just open `index.html` in any browser — that's it.

To serve it locally instead:

```bash
cd recipe-app
python3 -m http.server 8000   # then visit http://localhost:8000
```

> Nutrition values are approximate, per serving.
