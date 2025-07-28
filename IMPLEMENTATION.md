# Implementation Documentation

## Overview
This project is a job portal frontend built using modern web development tools and libraries. It provides a user-friendly interface for job seekers and administrators to interact with job postings, applications, and company profiles.

## Project Structure
The project is organized as follows:

```
job-portal-frontend/
├── public/                # Static assets
├── src/                   # Source code
│   ├── assets/            # Images and other assets
│   ├── components/        # React components
│   │   ├── admin/         # Admin-specific components
│   │   ├── auth/          # Authentication components
│   │   ├── shared/        # Shared components like Navbar and Footer
│   │   ├── ui/            # UI components like buttons, inputs, etc.
│   ├── hooks/             # Custom React hooks
│   ├── lib/               # Utility libraries
│   ├── redux/             # Redux slices and store
│   ├── utils/             # Utility functions and constants
├── package.json           # Project metadata and dependencies
├── tailwind.config.js     # Tailwind CSS configuration
├── vite.config.js         # Vite configuration
```

## Key Features

### User Features
- **Job Search**: Browse and filter job listings.
- **Profile Management**: Update user profiles.
- **Application Tracking**: View applied jobs and their statuses.

### Admin Features
- **Job Management**: Create, update, and delete job postings.
- **Company Management**: Manage company profiles and setup.
- **Applicant Tracking**: View and manage job applicants.

## Technologies Used

### Frontend
- **React**: For building the user interface.
- **React Router**: For client-side routing.
- **Redux Toolkit**: For state management.
- **Tailwind CSS**: For styling.
- **Radix UI**: For accessible UI components.

### Development Tools
- **Vite**: For fast development and build processes.
- **ESLint**: For linting and code quality.
- **PostCSS**: For CSS processing.

## Folder Details

### `src/components`
Contains reusable React components categorized into subfolders:
- **admin/**: Components for admin functionalities like job and company management.
- **auth/**: Components for login and signup.
- **shared/**: Common components like Navbar and Footer.
- **ui/**: Basic UI elements like buttons, inputs, and dialogs.

### `src/hooks`
Custom React hooks for fetching and managing data, such as:
- `useGetAllJobs`
- `useGetAppliedJobs`

### `src/redux`
Redux slices for managing application state:
- `applicationSlice.js`: Handles application-related state.
- `authSlice.js`: Manages authentication state.
- `companySlice.js`: Manages company-related state.
- `jobSlice.js`: Handles job-related state.

### `src/utils`
Utility functions and constants used across the project.

## How to Run the Project

1. **Install Dependencies**:
   ```bash
   npm install
   ```

2. **Start Development Server**:
   ```bash
   npm run dev
   ```

3. **Build for Production**:
   ```bash
   npm run build
   ```

4. **Preview Production Build**:
   ```bash
   npm run preview
   ```

## Contribution Guidelines

1. Fork the repository and create a new branch for your feature or bugfix.
2. Write clear and concise commit messages.
3. Ensure code quality by running:
   ```bash
   npm run lint
   ```
4. Submit a pull request with a detailed description of your changes.

## License
This project is licensed under the MIT License.
