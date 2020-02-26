# elasticsearchutils

Some command line sh wrappers around REST commands I find useful for ElasticSearch.

Some of them loop, giving you a little text based monitoring screen.

Set $ESCLUSTER in your environment to the URL you need to use.
Otherwise, will default to http://localhost:9200

* esgethealth - Overall health of cluster
* esgetsettings - Dump ALL the cluster settings to stdout
* esmoveshard - Usually a component in a script, to move multiple shards at a time
* esmoveshards - Move a fixed number of shards off one node to another node
* esnodeshards - List count of shards per node
* essetvalue - More easily set things like cluster.routing.allocation.exclude._ip 
* essetshardallocation - Convenience toggle for clusterside cluster.routing.allocation.enable value
