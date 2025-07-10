# Front-End of the Advertisement System – Unfinished School Project

## Description

This was my first larger-scale React application, so it may include some non-optimal practices or minor bugs. However, I focused on maintaining scalability and a well-organized code structure.

## Structure

### `assets`
Contains commonly used CSS files and images.

### `components`
Includes reusable components shared across most pages.

### `hooks`
Provides custom hooks for features like authentication, data fetching, and validation.

### `pages`
Holds page-level components, along with page-specific CSS and internal components.

### `services`

#### `api`
Services responsible for executing requests to the back-end.

#### `contexts`
Contexts and providers shared across multiple pages and subpages.

### `utils`
Utility scripts and helper functions.

## Commands

- `npm start` – starts the app locally and connects to the local back-end.
- `npm run deploy` – starts the app locally and connects to an external back-end (external service currently not deployed).

## Known Bugs

- Verification and password reset emails contain only a token instead of a full clickable link. The token needs to be manually pasted into: 'http://localhost:3000/register/verify/{token}'
  
