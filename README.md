# React Router v6 Catch-all Route Conflict

This repository demonstrates a common issue in React Router v6 related to the catch-all route (`/*`).  When a catch-all route is defined, it can unintentionally override other routes, preventing them from being matched correctly.

The `App.js` file shows the problematic code. The `AppSolution.js` demonstrates how to correctly use the catch all route.

## How to Reproduce

1. Clone this repository.
2. Install dependencies: `npm install`
3. Run the app: `npm start`
4. Observe that navigating to `/about` does not show the About component and the Not Found page renders instead.

## Solution

The solution involves carefully placing the catch-all route at the end of the route definitions.  The `AppSolution.js` shows the correct structure.