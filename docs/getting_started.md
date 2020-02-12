# Getting Started

## Docker-compose instructions

1. Clone the repo.

        git clone git@github.com:mnguyenngo/todoless.git

2. Build the docker image.

        docker-compose build

3. Run a container.

        docker-compose up

4. See the running containers. You will need to open a new terminal window.

        docker ps

5. Stop a container.

        docker stop <CONTAINER ID>

6. Stop all running containers.

        docker stop $(docker ps -q)

## Docker instructions

1. Clone the repo.

        git clone git@github.com:mnguyenngo/todoless.git

2. Build the docker image.

        docker build --tag todoless_api .

3. Run a container.

        docker run -d --name api -p 5000:80 todoless_api

4. See the running containers.

        docker ps

5. Stop a container.

        docker stop <CONTAINER ID>

6. Stop all running containers.

        docker stop $(docker ps -q)

## References

* [FastAPI Docker Image README](https://github.com/tiangolo/uvicorn-gunicorn-fastapi-docker)
* [FastAPI Deployment Docs](https://fastapi.tiangolo.com/deployment/)
