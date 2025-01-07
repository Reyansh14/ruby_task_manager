# Task Manager

A simple and elegant task management application built with Ruby on Rails. This application allows users to create, manage, and track tasks with due dates and completion status.

## Features

- Create new tasks with title, description, and due date
- Mark tasks as complete/incomplete
- Edit existing tasks
- Delete tasks
- View all tasks sorted by due date
- Clean, responsive user interface
- Visual feedback for completed tasks

## Technical Stack

- Ruby on Rails
- PostgreSQL
- HTML/ERB
- CSS
- Hotwire/Turbo

## Prerequisites

- Ruby 3.2.2
- Rails 7.1
- PostgreSQL

## Setup

1. Clone the repository:
```bash
git clone https://github.com/yourusername/task_manager.git
cd task_manager
```

2. Install dependencies:
```bash
bundle install
```

3. Setup the database:
```bash
rails db:create
rails db:migrate
```

4. Start the server:
```bash
rails server
```

5. Visit `http://localhost:3000` in your browser

## Project Structure

Key files and directories:

```
app/
├── controllers/
│   └── tasks_controller.rb    # Task CRUD operations
├── models/
│   └── task.rb               # Task model
├── views/
│   └── tasks/                # Task views
│       ├── _form.html.erb    # Shared form partial
│       ├── index.html.erb    # Tasks listing
│       ├── new.html.erb      # New task form
│       └── edit.html.erb     # Edit task form
└── assets/
    └── stylesheets/
        └── tasks.css         # Task-specific styles
```

## Database Schema

The `tasks` table includes:

- `title` (string): Task title
- `description` (text): Detailed task description
- `due_date` (datetime): Task deadline
- `completed` (boolean): Task completion status
- timestamps

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).
