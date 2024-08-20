# Helpdesk Ticket Management System

This Helpdesk Ticket Management System is a Laravel-based application integrated with Filament Admin. It allows users to submit tickets for questions, assistance requests, or issue reports. Admins can manage and prioritize tickets, track their history, and ensure that all issues are handled efficiently.

## Features

- **Ticket Submission**: Users can create and submit new tickets containing their questions, assistance requests, or issue reports.
- **Ticket Management**: Admins have the ability to view, assign, or close tickets submitted by users.
- **Ticket Prioritization**: Users can prioritize their tickets to highlight the urgency level.
- **History and Tracking**: The system records all activities and conversations within each ticket, providing a clear history for tracking and auditing purposes.

## User Roles

### 1. Super Admin
- **Email**: superadmin@example.com
- **Password**: password

### 2. Admin Unit
- **Email**: adminunit@example.com
- **Password**: password

### 3. Staff Unit
- **Email**: staffunit@example.com
- **Password**: password

### 4. General User
- **Email**: user@example.com
- **Password**: password

## Installation Guide

Follow these steps to get the project running on your local machine.

### Prerequisites

- PHP 8.0 or higher
- Composer
- Node.js and npm
- MySQL or any other database supported by Laravel
- Git

### Step 1: Clone the Repository

First, clone the repository from GitHub to your local machine:

```bash
git clone https://github.com/OnyangoOdipo/Helpdesk-with-Filament.git
cd Helpdesk-with-Filament
```

### Step 2: Install Dependencies

Run the following command to install PHP dependencies using Composer:

```bash
composer install
```

Next, install JavaScript dependencies using npm:

```bash
npm install
```

### Step 3: Set Up Environment Variables

Copy the `.env.example` file to `.env`:

```bash
copy .env.example .env
```

Open the `.env` file in a text editor and configure the database settings:

```dotenv
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=database name
DB_USERNAME=database username
DB_PASSWORD=database password
```

### Step 4: Generate Application Key

Generate the application key using the following Artisan command:

```bash
php artisan key:generate
```

### Step 5: Run Migrations and Seeders

Run the database migrations and seed the database:

```bash
php artisan migrate --seed
```

### Step 6: Compile Assets

Compile the front-end assets using Vite:

```bash
npm run dev
```

### Step 7: Serve the Application

Finally, serve the application locally:

```bash
php artisan serve
```

The application should now be running at `http://127.0.0.1:8000`.

## Usage

### Logging In

Use the credentials provided above to log in as different user roles.

### Ticket Submission

- General users can submit tickets via the "Submit Ticket" page.
- They can assign a priority level to each ticket to indicate the urgency.

### Ticket Management

- Admins and staff can view, assign, and close tickets.
- They can track the status and history of each ticket through the system.

### Ticket Prioritization

- Users can prioritize their tickets upon submission.
- Admins can re-prioritize tickets based on their assessment of the situation.

### History and Tracking

- All activities, including comments, status changes, and assignments, are logged and can be reviewed by users with appropriate permissions.

## Additional Information

### Filament Admin

This project utilizes Filament Admin for managing the backend. It provides a user-friendly interface for managing tickets, users, and other resources.

### Security

Ensure that you do not deploy the application in a production environment without configuring proper security measures such as HTTPS, environment variables, and access control.

## Contributing

If you'd like to contribute to this project, please fork the repository and submit a pull request. We welcome contributions of all kinds, including bug fixes, feature requests, and documentation improvements.