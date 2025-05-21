**How to build and run:**
We run the app only by the command: "docker-compose up":

1. app.py - the file prints how many times the page has been viewd
2. Dockerfile - for image building
3. Docker-Compose file - we will use Docker Compose to containerize the Redis Flask application - to launch the containers at once, as one application.
   In docker-compose.yml - we'll build the image from the dockerfile
4. The app is running!
5. The number of times the page has been viewed will be updated (each refresh increases the amount by 1) if the app stops running and restarts – because there is a volume defined in the docker-compose.yaml
6. Tag the image: docker tag simple-flask-redis-app:v1 dvirdock/simple-flask-redis-app:v1
7. Push: docker push dvirdock/simple-flask-redis-app:v1
8. A Docker image published on Docker Hub: [https://hub.docker.com/repository/docker/dvirdock/simple-flask-redis-app/tags/v1/sha256-c16b8c89b8308dc075417e97ebc393b60732eda78dc67a3e841ad101df928ddf
](url)
