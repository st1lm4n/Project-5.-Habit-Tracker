# Habit Tracker

Full-featured habit tracking application with scheduled notifications.

## Features

- User authentication
- Habit management
- Periodic notifications
- Background tasks
- Scheduled jobs

## Tech Stack

Python
Django
PostgreSQL
Redis
Celery
Celery Beat
Docker

## Architecture
                    User
                      │
                      ▼
                 Django App
                      │
                      ▼
                 PostgreSQL
                      │
                      │
        ┌─────────────┴─────────────┐
        ▼                           ▼
      Celery                      Redis
        │
        ▼
    Notifications
        │
        ▼
    Celery Beat
