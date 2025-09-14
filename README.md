# DJS02 – Web Component: Podcast Preview

## Overview

In this project, I builT a reusable and encapsulated **custom HTML element** that displays a podcast preview. The component follows the **Web Component standard**, using `customElements.define()` and works independently from the main application logic. This component enhances modularity, promotes reuse, and reduces code duplication across the app.

The component is designed to **accept podcast data via attributes or properties**, displays relevant UI elements (such as title, cover image, and genres), and **communicates with the main application** through custom events.

--- 

### Web Component Functionality

- I Created a **custom HTML element** using `customElements.define()`.
- Accepts data (cover image, title, genres, number of seasons, and last updated date) **as attributes or properties**.
- Keeps the component **stateless** and reliant on external data provided by the parent.
- Uses **Shadow DOM** for style and logic encapsulation to avoid global conflicts.
- It triggers a **custom event** when a user interacts with the component (e.g., clicking), so that the parent application can open a modal or take other actions without tightly coupling to the component’s logic.

--- 

- The component renders a clean and **visually consistent preview** of each podcast.
- Displays:
  - Podcast **cover image**
  - Podcast **title**
  - **Genre names**
  - **Number of seasons**
  - **Last updated** in a human-readable format
- The component is **responsive**, and matches the overall app design on desktop and mobile.
- On click, the component notifies the parent app to **open a modal** or navigate to details.

---