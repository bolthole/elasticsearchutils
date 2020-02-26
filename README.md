# elasticsearchutils

Some command line sh wrappers around REST commands I find useful for ElasticSearch.

Some of them loop, giving you a little text based monitoring screen.

Set $ESCLUSTER in your environment to the URL you need to use.
Otherwise, will default to http://localhost:9200

* essetvalue - more easily set things like cluster.routing.allocation.exclude._ip 
* essetshardallocation - convenience toggle for clusterside cluster.routing.allocation.enable value
* esgethealth - overall health of cluster
* esmoveshard - Usually a component in a script, to move multiple shards at a time
* esgetsettings - dump ALL the cluster settings to stdout
* esnodeshards - list count of shardes per node
