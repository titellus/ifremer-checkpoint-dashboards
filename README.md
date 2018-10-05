# Checkpoint dashboards

This repository contains the Talend jobs to export from Checkpoint metadata records quality indicators.
Indicators are then available in different format:
* Excel table
* CSV files
* SQLite db
* Elasticsearch index

Then Kibana is used to analyze this information.


## Dependencies

* Elasticsearch 6.4.x
* Kibana 6.4.x
* Talend open studio 6.2.x

## Manage index

Creation:
```
curl -X PUT -H "Content-Type:application/json" http://localhost:9200/checkpoint -d @checkpoint.json
```

Removal:
```
curl -X DELETE http://localhost:9200/checkpoint
```


## Data adequacy report visualizations

### Annex 1: List of components

See [screenshot](img/annex1-list-of-components.png).

![](img/annex1-list-of-components.png?raw=true)

### Annex 3: P02 quality measures


See [screenshot](img/annex2-p02-quality-measures.png).

![](img/annex2-p02-quality-measures.png?raw=true)

### Annex 5: Components statistics


See [screenshot](img/annex5-components-statistics.png).

![](img/annex5-components-statistics.png?raw=true)

### Quality measures by challenges

See [screenshot](img/quality-measures-by-challenges.png).


![](img/quality-measures-by-challenges.png?raw=true)



