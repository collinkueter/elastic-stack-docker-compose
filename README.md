# elastic-stack-docker-compose

## To Run ElasticSearch Individually

`docker container run -it -p 9200:9200 -p 9300:9300 elasticsearch:v0.1`

### Test If ElasticSearch is Working

Create an index
`curl -X PUT "localhost:9200/customer?pretty"`
View Indexes
`curl -X GET "localhost:9200/_cat/indices?v"`
Put Data in index
`curl -X PUT "localhost:9200/customer/_doc/1?pretty" -H 'Content-Type: application/json' -d'{"name": "John Doe"}'`
View Data
`curl -X GET "localhost:9200/customer/_doc/1?pretty"`

## To Run Logstash Individually

`docker container run -it -p 9200:9200 logstash:v0.2`

### Test If Logstash is Working

type `Hello` or anything into the console and it will be spit back out
Also: `curl -X GET "localhost:9200/_cat/health?v"`