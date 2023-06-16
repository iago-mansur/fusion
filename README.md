docker-compose down

mkdir fusion

cd fusion

code .

criar Dockerfile, docker-compose.yml, requirements.txt, .gitignore, pasta project

sudo chmod 666 /var/run/docker.sock

docker build .

docker-compose build

docker-compose run --rm app sh -c "django-admin startproject fusion ."

docker-compose up

http://127.0.0.1:8000/


CRTL^C

carregar pasta template

docker-compose build

docker-compose run --rm app sh -c "django-admin startapp core"

pip install django psycopg2-binary gunicorn dj-static django-stdimage
pip freeze > requirements.txt

editar settings.py

criar pasta core.templates, core.static

editar urls.py

criar core.urls.py


criar app/core/management/init.py

app/core/management/commands/init.py

criar app/core/management/commands/wait_for_db.py


docker-compose run --rm app sh -c "python manage.py test"

docker-compose run --rm app sh -c "python manage.py wait_for_db"


editar Dockerfile

editar docker-compose.yml
DB_HOST=db vs 'localhost'?

docker-compose down

docker-compose up

http://127.0.0.1:8000/






editar core.views.py

criar contato.html index.html produto.html

criar pastas: css, js, images

crair arquivo js.





