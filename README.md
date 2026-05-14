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

## Production Deployment Notes

The `docker-compose.prod.yaml` file is used on the EC2 instance.

currently the docker compose file is pulling the image from my own ECR.
If you wish to pull the image from your ECR, change the aws credentials inside the  `docker-compose.prod.yaml` file.
