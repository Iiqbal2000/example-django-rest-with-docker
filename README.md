# example-django-rest-with-docker

Contoh konfigurasi ada di file masing2

build dengan docker compose:
docker-compose run web django-admin startproject namaproject .

ganti grup:
sudo chown -R $USER:$USER .

migrations dan create super user:
docker-compose run --services-ports web python manage.py migrate
docker-compose run --service-ports web python manage.py createsuperuser

init db:
docker-compose up -d db

init web:
docker-compose up -d web
