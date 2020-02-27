# elasticsearchutils

Some command line sh wrappers around REST commands I find useful for ElasticSearch.

Some of them loop, giving you a little text based monitoring screen.

Set $ESCLUSTER in your environment to the URL you need to use.
Otherwise, will default to http://localhost:9200

* esgethealth - Display overall health of cluster
* esgetsettings - Dump ALL the cluster settings to stdout
* esgettemplates - Get templated values for indexes
* esmoveshard - Move ONE shard from one node to another. Mostly just a component of esmoveshards.
* esmoveshards - Move a fixed number of shards off one node to another node
* esnodeshards - Display per-node shards info. Use -v for details
* essetvalue - More easily set things like cluster.routing.allocation.exclude._ip 
* essetshardallocation - Convenience toggle for clusterside cluster.routing.allocation.enable value


Sample output from esnodeshards -v:

   ...Querying...     NORM  INIT RELOC
       sysdata01-cor  1038            
       sysdata02-cor  1228           3
       sysdata03-cor  1038            
       sysdata04-cor  1188     2     
       sysdata05-cor  1036            
       sysdata06-cor  1212           5
       sysdata07-cor  1035           1
       sysdata08-cor  1220           7
       sysdata09-cor  1037            
       sysdata10-cor   181     1      
       sysdata11-cor     8            
       sysdata12-cor  1198            
       sysdata13-cor  1036            
-- UNASSIGNED == 0
