# 🍲 Forkify // Recipe Search & Meal Planning SPA

A responsive Single Page Application (SPA) designed for searching over 1,000,000 recipes, adjusting ingredient servings dynamically, bookmarking favorites, and uploading custom user-generated recipes to a third-party API.

---

## 🚀 Key Features

* **Recipe Search & Pagination:** Real-time recipe lookups with client-side paginated results.
* **Serving Adjustment Calculator:** Automatically updates ingredient proportions when changing the number of servings.
* **Persistent Bookmarking:** Saves favorite recipes to `localStorage` for uninterrupted access across sessions.
* **Custom Recipe Uploads:** Interactive modal form supporting ingredient validation and direct API publication.
* **Fractional Quantity Formatting:** Clean display of cooking measurements and units.

---

## 🏗️ Architecture & Engineering Patterns

The application is structured strictly according to the **Model-View-Controller (MVC)** architectural pattern to decouple business logic from the UI:

* **Model (`src/js/model.js`):** Manages API queries, recipe state objects, bookmarks, and `localStorage` synchronization.
* **Views (`src/js/views/`):** Dedicated view classes (e.g., `recipeView`, `searchView`, `resultsView`, `paginationView`, `bookmarksView`, `addRecipeView`) implementing Publisher-Subscriber patterns.
* **Controller (`src/js/controller.js`):** Handles application events, intercepts user inputs, and orchestrates data flow between the Model and Views.

---

## 🛠️ Tech Stack

* **Core:** Modern Vanilla JavaScript (ES6+ Modules, Async/Await, Classes)
* **Styling:** Sass / SCSS (BEM methodology)
* **Bundler & Tooling:** Parcel / Webpack, Babel
* **API Integration:** Forkify REST API

---

## 💻 Local Development Setup

```bash
# 1. Clone the repository
git clone [https://github.com/jaroslawzawadzki/forkify-cours-jz.git](https://github.com/jaroslawzawadzki/forkify-cours-jz.git)
cd forkify-cours-jz

# 2. Install project dependencies
npm install

# 3. Start local development server
npm start

# 4. Create a production build
npm run build
