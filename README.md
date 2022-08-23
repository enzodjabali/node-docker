# node-docker

Start :
docker-compose -f docker-compose.yml -f docker-compose.dev.yml up -d

Start and build a new docker image (useful in production environment):
docker-compose -f docker-compose.yml -f docker-compose.prod.yml up -d --build

Stop :
docker-compose -f docker-compose.yml -f docker-compose.dev.yml down -v

Access MongoDB :
docker exec -it node-docker_mongo_1 mongo -u "admin" -p "1234"