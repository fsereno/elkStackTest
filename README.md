https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html

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

POST /products/_doc/200
{
  "name":"My product with ID specified",
  "cost": 11.99
}

POST /products/_update/200
{
  "doc": {
    "cost": 100.99
  }
}

PUT /products/_doc/200
{
  "name":"Updated product name with PUT",
  "cost": 111.99
}

GET /products/_doc/200

GET /products

GET /_cluster/health

GET _search
{
  "query": {
    "match_all": {}
  }
}