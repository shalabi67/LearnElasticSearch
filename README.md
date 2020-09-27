# LearnElasticSearch

## Rest API

### cluster
- http://localhost:9200/
- http://localhost:9200/_cat/health?v&pretty
- http://localhost:9200/_cat/nodes?v&pretty

### Indices
#### commands
- PUT means we want to create the index and add documents
- POST means we want to add a document

#### APIs
- http://localhost:9200/_cat/indices?v&pretty
- curl -X PUT http://localhost:9200/products?pretty
- curl -d @json/product.json -H "Content-Type: application/json" -X PUT http://localhost:9200/products/mobiles/1?pretty
`products is the index. 
mobiles is the document type.`

- curl -d @json/product.json -H "Content-Type: application/json" -X POST http://localhost:9200/products/mobiles?pretty
- curl http://localhost:9200/products/mobiles/1?pretty

