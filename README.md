mkdir fusion

cd fusion

code .

criar Dockerfile, docker-compose.yml, requirements.txt, .gitignore, pasta project

sudo chmod 666 /var/run/docker.sock

docker build .

docker-compose build

docker-compose run --rm app sh -c "django-admin startproject app ."

docker-compose up

http://127.0.0.1:8000/