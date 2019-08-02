# docker-flask
It is part of a little course I took of Flask, a Python framework. I mixed it with a guide to learn Docker and Docker compose.

## Flask sources:
- https://www.udemy.com/intro-to-flask/
- https://flask.palletsprojects.com/en/1.1.x/quickstart/
- https://flask-sqlalchemy.palletsprojects.com/en/2.x/

## Docker sources:
- https://docker-curriculum.com/
- https://www.youtube.com/watch?v=YFl2mCHdv24
- https://www.youtube.com/watch?v=Qw9zlE3t8Ko
- https://nickjanetakis.com/blog/tag/docker-tips-tricks-and-tutorials
- https://docs.docker.com/engine/reference/builder/
- https://docs.docker.com/compose/compose-file/#compose-and-docker-compatibility-matrix

## How to run
- Build project.
```
docker-compose up
```

- Enter to the project container and open python console then create the table.
```
docker ps -a
docker exec -it CONTAINER_ID_HERE bash
python
from app import db
db.create_all()
```

- Done, the site loads on localhost:5000
