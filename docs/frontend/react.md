# React Frontend Overview

The frontend is built with **React 19** and **TailwindCSS**.  
It focuses on a clean component-driven architecture and performance.

## Folder Structure

frontend/
├── components/ # Reusable UI components
├── pages/ # Page-level components
├── hooks/ # Custom React hooks
├── context/ # React Context providers
└── assets/ # Images, icons, styles


## Components

### TaskCard
Displays individual task information and supports drag-and-drop interactions.

### TaskList
Renders a list of TaskCards and supports filtering by status.

### NavigationBar
Top navigation component with links to Dashboard, Profile, and Settings.

## Routing

- Implemented using **React Router v6**
- Nested routes for Dashboard, Task Details, and User Profile

## API Integration

- **React Query** is used to fetch and cache API data
- Handles error states and loading indicators automatically


