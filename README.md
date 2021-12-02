# elkStackTest
A sandbox for all things ELK Stack, will run in containers using Docker.

## Commands
docker compose up

then go to:

http://localhost:5601/app/dev_tools#/console

PUT /products

POST /products/_doc
{
  "name":"My second product",
  "cost": 10.99
}

GET /products/_doc/jY0pfH0BuPOXiMGxHfER

GET /_cluster/health

GET _search
{
  "query": {
    "match_all": {}
  }
}