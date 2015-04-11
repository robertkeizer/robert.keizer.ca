---
layout:		post
title:		PouchDB Quorum Plugin
summary:	I'm starting a plugin that provides quorum functionality for PouchDB! 
category:	pouchdb-quorum
---

### Some Background

I really like [PouchDB](http://pouchdb.com/) and [CouchDB](http://couchdb.apache.org) for replication [[1]](http://docs.couchdb.org/en/1.6.1/replication/intro.html) [[2]](http://pouchdb.com/api.html#replication). CouchDB [version 2.0](https://couchdb.apache.org/developer-preview/2.0/) by default comes in a clustered system, with multiple instances running on different ports ( `15984`, `25984`, `35984` ). 

These provide for per database replication and availability ( I think, it may be all databases on a node ). Either way, the level of redundancy is more than many applications require. For larger clusters of data, this becomes impractical.

### The Quorum Plugin

The quorum plugin is designed to be flexible enough to handle writing data to x of y databases, using replication without any change to the PouchDB interaction, apart from some configuration on initial setup.

The plugin is being designed with high availability in mind. While some performance optimizations may be put in place, emphasis will be focused on ensuring reliability.

Once the plugin is functional and stable, additional features planned include:

  * Adding and removing nodes
  * Re-balancing existing data
  * Changing the level of redundancy in runtime

[https://github.com/robertkeizer/pouchdb-quorum](https://github.com/robertkeizer/pouchdb-quorum)
