# Quicksell-Frontend-assignment
A dynamic Kanban Board application built using ReactJS and Redux for state management. The app allows users to group tickets by status, user, or priority and sort them dynamically while persisting the state across page reloads.

Features
Dynamic Grouping:

Group tickets by:
Status: To-Do, In Progress, Done, and Canceled.
User: Assigned users.
Priority: Urgent, High, Medium, Low, and No Priority.
State Management:

Centralized state management using Redux.
Actions for grouping and sorting tickets.
Reducer logic for managing and updating grouped tickets.
Sorting Options:

Sort tickets within groups by:
Priority: Descending order.
Title: Alphabetical order.
Persistent State:

The selected grouping and sorting options persist across page reloads using localStorage.
Custom Styling:

Pure CSS for responsive and visually appealing layouts.
SVG icons integrated for priorities, statuses, and other UI elements.
Screenshots
1. Grouping by Status

2. Grouping by User

3. Grouping by Priority

4. Ticket Card

Folder Structure
perl
Copy code
src/
├── Actions/
│   ├── DataAction.js          # Redux actions for grouping and sorting
├── components/
│   ├── Card/
│   │   ├── Card.css           # Styles for TicketCard
│   │   ├── Card.jsx           # Component for individual tickets
│   ├── DashBoard/
│   │   ├── DashBoard.css      # Styles for Kanban board layout
│   │   ├── DashBoard.jsx      # Main Kanban board component
│   ├── Loading/
│   │   ├── Loading.jsx        # Loading spinner or placeholder
│   ├── NavBar/
│       ├── NavBar.css         # Styles for navigation bar
│       ├── NavBar.jsx         # Top navigation bar component
├── Reducers/
│   ├── DataReducer.js         # Redux reducer for data management
├── App.css                    # Global app styles
├── App.js                     # Main application entry point
├── index.js                   # Entry file for React DOM rendering
├── store.js                   # Redux store configuration

Getting Started
1. Prerequisites
Node.js (v14 or higher)
npm (comes with Node.js)
2. Installation
Clone the repository:

bash
Copy code
git clone <repository-url>
cd kanban-board
Install dependencies:

bash
Copy code
npm install
Start the development server:

bash
Copy code
npm start
The application will be available at http://localhost:3000.

Usage
Group Tickets:

Use the dropdown in the NavBar to group tickets by status, user, or priority.
Sort Tickets:

Within each group, sort tickets by priority (default) or title.
Persistent State:

The app automatically saves your selected grouping and sorting options.
Built With
ReactJS: Frontend framework for building the UI.
Redux: Centralized state management.
Pure CSS: Custom styles for all components.
SVG Icons: Used for priorities and statuses.
Redux Overview
Actions (Actions/DataAction.js)
groupTickets(criteria): Dispatches an action to group tickets by the specified criteria (status, user, priority).
sortTickets(criteria): Dispatches an action to sort tickets within groups by the specified criteria (priority or title).
Reducer (Reducers/DataReducer.js)
Manages:
Tickets: The raw ticket data.
Grouped Tickets: Tickets grouped by the selected criteria.
Grouping: Current grouping option.
Sorting: Current sorting option.
Store (store.js)
Configures Redux store with the DataReducer.
Deployment
Build the production-ready app:

bash
Copy code
npm run build
Deploy the build/ directory to any hosting service:

Netlify
Vercel
GitHub Pages
License
This project is licensed under the MIT License - see the LICENSE file for details.




© 2024 Begari Balaraj



