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

editar settings.py

criar pasta core.templates, core.static

editar urls.py

criar core.urls.py


criar app/core/management/init.py

app/core/management/commands/init.py

criar app/core/management/commands/wait_for_db.py

editar Dockerfile

editar docker-compose.yml
DB_HOST=db vs 'localhost'?

docker-compose down

docker-compose up

http://127.0.0.1:8000/



editar core.views.py, urls.py

criar arquivos html em core.templates

transferir arquivos estáticos para core.static

docker-compose up

http://127.0.0.1:8000/

docker-compose down

Editar core.models.py, admin.py, core.views.py

Criar core.forms.py

Editar settings.py


sudo chmod 666 /var/run/docker.sock

docker-compose build

docker-compose run --rm app sh -c "pip install model_mommy coverage"

pip freeze

atualizar requirements.txt

coverage run manage.py test

coverage report

coverage html

cd htmlcov

python -m http.server

rm -rf htmlcov

coverage run manage.py test

cd htmlcov

python -m http.server