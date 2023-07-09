# Cinema Service API

API service for cinema management written on DRF

## Installing using GitHub:

Install PostgresSQL and create db
```
git clone git@github.com:MKeSiMu/cinema-service-api.git
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
set DB HOST=<your db hostname>
set DB NAME=<your db name>
set DB USER=<your db username>
set DB PASSWORD=<your db user password>
set SECRET KEY=<your secret key>
python manage.py migrate
python manage.pyrunserver
```
## Run with docker:

```
docker-compose build
docker-compose up
```

## Getting access:

- create user via /api/user/register
- get access token via /api/user/token

## Features:

- JWT authenticated
- Admin panel /admin/
- Documentation is located at /api/doc/swagger
- Managing orders and tickets
- Creating movies with genres, actors
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie sessions

