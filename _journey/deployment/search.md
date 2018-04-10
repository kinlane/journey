---
class:
- line
rel:
- self
properties:
  name: Search
  sort: 1131
  level: 2
  description: Leveraging search services and tooling to index and make existing resources
    accessible, allowing for documents, structured, and unstructured data to be deployed
    as web APIs.
  tools:
    - name: Elasticsearch
      description: Elasticsearch is a distributed RESTful search engine built for the cloud.
      url: https://github.com/elastic/elasticsearch
    - name: Apache Solr
      description: Solr is the popular, blazing-fast, open source enterprise search platform built on Apache Lucene.
      url: http://lucene.apache.org/solr/    
  service:
    - name: Elasticsearch
      description: Elasticsearch is a search engine based on Lucene. It provides a distributed, multitenant-capable full-text search engine with an HTTP web interface and schema-free JSON documents.
      url: https://www.elastic.co/           
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Search
  links:
  - rel:
    - self
    href: deployment/search/
  - rel:
    - parent
    href: deployment/
links:
- rel:
  - self
  href: deployment/search/
- rel:
  - parent
  href: deployment/
...
