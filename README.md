# Shopping List App
A simple shopping list app built with React that lets you quickly search through items and mark them as completed. The focus of this project is clean state management, responsive UI updates, and keeping the app fast and predictable without using any build tools.

## Features
- Live search that works as you type
- Case-insensitive and partial text matching
- Checkboxes to mark items as done
- Selected items are crossed out visually
- Smooth performance using memoization
- Responsive, minimal UI

## Tech Stack
- React (via CDN)
- ReactDOM
- Babel (for in-browser JSX)
- HTML
- CSS

## Project Structure
- `index.html` – Loads React, Babel, and mounts the app
- `index.jsx` – Main application logic and components
- `styles.css` – Styling and layout

## How It Works
The search input is controlled using React state. Items are filtered based on the current query, and the filtering logic is memoized so it only re-runs when the search value changes. Selected items are stored in state and toggled on and off using a single handler, with visual feedback applied directly in the list.

## Running the App
You can run this app by opening `index.html` in the browser.  
For the best experience, use a local server (for example, VS Code Live Server).

## Notes
This project uses React via CDN instead of a bundler to keep things lightweight and easy to inspect. Console logs are included to demonstrate when memoized logic and callbacks are re-created.
