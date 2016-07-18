# Latest ElasticSearch 

With minor changes in elasticsearch.yml

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

should output something like this.

```
{
  "name" : "node-1",
  "cluster_name" : "elasticsearch-cors",
  "version" : {
    "number" : "2.3.4",
    "build_hash" : "e455fd0c13dceca8dbbdbb1665d068ae55dabe3f",
    "build_timestamp" : "2016-06-30T11:24:31Z",
    "build_snapshot" : false,
    "lucene_version" : "5.5.0"
  },
  "tagline" : "You Know, for Search"
}
```
