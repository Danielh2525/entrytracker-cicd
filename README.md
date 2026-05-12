# EntryTracker

EntryTracker is a simple Flask + MySQL application that tracks page visits.

## Architecture

The application runs as a 2-tier Docker Compose app:

- Flask web application
- MySQL database
- Docker network
- Docker volume
- Health check

all required env variables can be found in .env.example
