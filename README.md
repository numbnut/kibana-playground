## Startup platform
```
docker-compose up -d
```

## Write data to Elasticsearch
```
curl -XPOST 'localhost:9200/monitoring/temp/_bulk?pretty' --data-binary "@temperatur.json"
```

## Kibana Config
* Set index to `monitoring`

## Timelion
* Set time range from `2000-01-01 01:00:00` to `2000-01-01 01:10:00`
* Do the following query `.es(metric="avg:value")`
