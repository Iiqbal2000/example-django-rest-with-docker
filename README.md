# example-django-rest-with-docker

### Contoh konfigurasi ada di file masing-masing.

##### :horse: Build dengan docker compose :
```bash
docker-compose run web django-admin startproject namaproject
```

##### :dog: Ganti kepemilikan grup grup :
```bash
sudo chown -R $USER:$USER
```

##### :snake: Migrations dan create super user :
```bash
docker-compose run --services-ports web python manage.py migrate
docker-compose run --service-ports web python manage.py createsuperuser
```

##### :water_buffalo: Init db :
```bash
docker-compose up -d db
```

##### :cat2: Init web :
```bash
docker-compose up -d web
```

##### :dragon_face: Run server :
```bash
docker-compose up
```

##### :boom: Run bash :
```bash
docker-compose run web bash
```
