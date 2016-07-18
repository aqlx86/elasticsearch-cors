# Latest ElasticSearch with 

## Current settings

```
cluster.name: "elasticsearch-cors"
node.name: "node-1"
network.host: 0.0.0.0
http.port: 9200
http.cors.enabled: true
http.cors.allow-origin: "*"
```

## Usage

```
> docker pull aqlx86/elasticsearch-cors 
> docker run -d -p 9200:9200 -p 9300:9300 aqlx86/elasticsearch-cors
```

# Test

` curl localhost:9200 `
