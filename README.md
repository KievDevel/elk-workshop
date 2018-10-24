## Elastic workshop

Tutorial, describing main features of elasticsearch and some internal parts.

**Conents:**
1. Basic operations
2. Search
3. Filtering, sorting, grouping aggregations
4. Healthchecks
6. Search engines theory
7. Clusters, nodes, shards

**Run application:** `docker-compose up -d`

"VM - port", all accessible at localhost:
1. Portainer - 15000;
2. Kibana - 5601;
3. Logstash - 9600;
4. Elasticsearch - 9200;

**To add sample data run:**  curl -H "Content-Type: application/json" -XPOST "localhost:9200/bank/_doc/_bulk?pretty&refresh" --data-binary "@sampleAccounts.json"

*To get all of the workshop commands - copy-n-paste kibanaTutorial content into kibana dev tools.*

Some useful links:
1. [Docker setup for ELK](https://github.com/deviantony/docker-elk)
2. [Speed up elasticsearch](https://www.elastic.co/videos/speed-is-key-elasticsearch-under-the-hood)
3. [Getting started with elasticsearch](https://www.elastic.co/webinars/getting-started-elasticsearch?baymax=rtp&elektra=docs&storm=top-video&iesrc=ctr)

TODOs:
1. Explain analyzers
2. More info on filtering
3. Nested queries
4. Visualization

