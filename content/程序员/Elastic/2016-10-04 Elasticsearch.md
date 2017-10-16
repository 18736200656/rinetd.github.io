---
title: Awesome Elasticsearch
date: 2016-10-04T04:15:26+08:00
update: 2016-10-04 04:15:26
categories:
tags:
---

http://elasticsearch-cheatsheet.jolicode.com/


如果是按日期索引的日志，那么最好定期清除旧索引：
` curl -XDELETE -u <USER>:<PASSWORD> http://<HOST>:9200/logstash-$(date -d '-10days' +'%Y.%m.%d')`



#elasticsearch资源汇总

[awesome-elasticsearch](https://github.com/dzharii/awesome-elasticsearch)

[插件汇总](http://my.oschina.net/secisland/blog/636213)

[ES权威指南中文](http://es.xiaoleilu.com/)

[ES权威指南英文](https://www.elastic.co/guide/en/elasticsearch/guide/current/getting-started.html)

[ES安全search-guard](https://github.com/floragunncom/search-guard)

[elasticsearch相关介绍](http://www.searchtech.pro/)

[solr和elasticsearch对比](https://thinkbiganalytics.com/solr-vs-elastic-search/)

##ES管理

[bigdesk](https://github.com/lukas-vlcek/bigdesk)

##容器化

[elasticsearch-cloud-kubernetes](https://github.com/fabric8io/elasticsearch-cloud-kubernetes)

[Docker Official Image packaging for elasticsearch](https://github.com/docker-library/elasticsearch)

##剖析Elasticsearch集群系列

* [英文原文](http://insightdataengineering.com/blog/elasticsearch-crud/)

* [剖析Elasticsearch集群系列第一篇 存储模型和读写操作](http://www.infoq.com/cn/articles/analysis-of-elasticsearch-cluster-part01?utm_campaign=rightbar_v2&utm_source=infoq&utm_medium=articles_link&utm_content=link_text)

* [剖析Elasticsearch集群系列第二篇 分布式的三个C、translog和Lucene段](http://www.infoq.com/cn/articles/anatomy-of-an-elasticsearch-cluster-part02)

* [剖析Elasticsearch集群系列第三篇 近实时搜索、深层分页问题和搜索相关性权衡之道](http://www.infoq.com/cn/articles/anatomy-of-an-elasticsearch-cluster-part03?utm_campaign=rightbar_v2&utm_source=infoq&utm_medium=articles_link&utm_content=link_text)

* [nested 和parent使用介绍](https://segmentfault.com/a/1190000002803966)

##企业使用案例

* [使用Akka、Kafka和ElasticSearch等构建分析引擎](http://www.infoq.com/cn/articles/use-akka-kafka--build-analysis-engine?utm_source=infoq&utm_medium=related_content_link&utm_campaign=relatedContent_articles_clk)

* [用Elasticsearch构建电商搜索平台，一个极有代表性的基础技术架构和算法实践案例](http://chuansong.me/n/690173551706)

* [用Elasticsearch+Redis构建投诉监控系统，看Airbnb如何保证用户持续增长](http://h2ex.com/1584)

* [亿级规模的Elasticsearch优化实战](http://mp.weixin.qq.com/s?src=3&timestamp=1474505854&ver=1&signature=cOaIC8LeZ7x1h-8*nR35Gib7vU*ibCzA8SSURam4gu2WI2rgkj7ApGNQrqPzJT1sHZH3b5oZ5qEHTYQqA9MHw3PcGwY8C8972omkPQ2S*2cVnUuf3uzCuOglRm*YNG0CFbayLnEPihE8*AUgYb*MPA==)

* [Elasticsearch作为时间序列数据库](http://blog.csdn.net/jiao_fuyou/article/details/49663687)

# 索引原理

[ES原理](http://www.shaheng.me/blog/2015/06/elasticsearch--.html)

[ES analyzer](http://mednoter.com/all-about-analyzer-part-one.html)

[docvalues 介绍](http://qindongliang.iteye.com/blog/2297280)

[ElasticSearch存储文件解析](https://www.elastic.co/blog/found-dive-into-elasticsearch-storage)
#问题解决

[如何防止elasticsearch的脑裂问题](https://segmentfault.com/a/1190000004504225)

[9 Tips on ElasticSearch Configuration for High Performance](https://www.loggly.com/blog/nine-tips-configuring-elasticsearch-for-high-performance/)




# Awesome Elasticsearch

#### ← [Awesome TypeScript](https://github.com/dzharii/awesome-typescript) -= Awesome Elasticsearch =-
[![](https://raw.githubusercontent.com/dzharii/awesome-elasticsearch/master/awesome-elastic-logo.png)](https://github.com/dzharii/awesome-elasticsearch)

# General
## Elastic Stack
* [Elasticsearch](https://www.elastic.co/) official website
* [Logstash](https://www.elastic.co/products/logstash) is a data pipeline that helps you process logs and other event data from a variety of systems
* [Kibana](https://www.elastic.co/products/kibana) is a data analysis tool that helps to visualize your data; [Kibana Manual docs](https://www.elastic.co/guide/en/kibana/current/discover.html)
* [beats](https://www.elastic.co/products/beats) is the platform for building lightweight, open source data shippers for many types of data you want to enrich with Logstash, search and analyze in Elasticsearch, and visualize in Kibana.

## Open-source and free products, based on Elasticsearch
* [Yelp/elastalert](https://github.com/yelp/elastalert) is a modular flexible rules based alerting system written in Python
* [exceptionless/Exceptionless](https://github.com/exceptionless/Exceptionless) is an error (exceptions) collecting and reporting server with client bindings for a various programming languages
* [searchkit/searchkit](https://github.com/searchkit/searchkit) is a UI framework based on React to build awesome search experiences with Elasticsearch

## Elasticsearch developer tools and utilities

### Development and debugging
* [Sense (from Elastic)](https://github.com/elastic/sense/#sense) A JSON aware developer console to ElasticSearch; official and very powerful
* [Sense (Google Chrome extension)](https://chrome.google.com/webstore/detail/sense-beta/lhjgkmllcaadmopgmanpapmpjgmfcfig?hl=en) A JSON aware developer console to ElasticSearch; unofficial but very powerful
* [ES-mode](https://github.com/dakrone/es-mode) An Emacs major mode for interacting with Elasticsearch (similar to Sense)
* [Elasticsearch Cheatsheet](http://elasticsearch-cheatsheet.jolicode.com/) Examples for the most used queries, API and settings for all major version of Elasticsearch
* [Elasticstat](https://github.com/objectrocket/elasticstat) CLI tool displaying monitoring informations like htop

### Import and Export
* [Knapsack plugin](https://github.com/jprante/elasticsearch-knapsack)  is an "swiss knife" export/import plugin for Elasticsearch
* [Elasticsearch-Exporter](https://github.com/mallocator/Elasticsearch-Exporter) is a command line script to import/export data from ElasticSearch to various other storage systems
* [esbulk](https://github.com/miku/esbulk) Parallel elasticsearch bulk indexing utility for the command line.
* [elasticdump](https://github.com/taskrabbit/elasticsearch-dump) - tools for moving and saving indicies

## Elasticsearch plugins
### Cluster
* [sscarduzio/elasticsearch-readonlyrest-plugin](https://github.com/sscarduzio/elasticsearch-readonlyrest-plugin) Safely expose Elasticsearch REST API directly to the public
* [appbaseio/dejaVu](https://github.com/appbaseio/dejaVu/tree/dev) A modern, open-source data browser for Elasticsearch; [landing page](https://appbaseio.github.io/dejaVu/)  
* [mobz/elasticsearch-head](https://github.com/mobz/elasticsearch-head) is a powerful and essential plugin for managing your cluster, indices and mapping
* [Bigdesk](http://bigdesk.org/) - Live charts and statistics for elasticsearch cluster
* [Elastic HQ](http://www.elastichq.org/) - Elasticsearch cluster management console with live monitoring and beautiful UI
* [Kopf](https://github.com/lmenezes/elasticsearch-kopf) - Another management plugin that have REST console and *manual* shard allocation
* [Search Guard](https://github.com/floragunncom/search-guard) - Elasticsearch security for free

### Other
* [SIREn Join Plugin for Elasticsearch](https://github.com/sirensolutions/siren-join) This plugin extends Elasticsearch with new search actions and a filter query parser that enables to perform a "Filter Join" between two set of documents (in the same index or in different indexes).

### Integrations and SQL support
* [NLPchina/elasticsearch-sql](https://github.com/NLPchina/elasticsearch-sql/) - Query elasticsearch using familiar SQL syntax. You can also use ES functions in SQL.
* [elastic/elasticsearch-hadoop](https://github.com/elastic/elasticsearch-hadoop) - Elasticsearch real-time search and analytics natively integrated with Hadoop (and Hive)
* [jprante/elasticsearch-jdbc](https://github.com/jprante/elasticsearch-jdbc) - JDBC importer for Elasticsearch

### You know, for search
* [jprante/elasticsearch-plugin-bundle](https://github.com/jprante/elasticsearch-plugin-bundle) A plugin that consists of a compilation of useful Elasticsearch plugins related to indexing and searching documents

## Kibana plugins and applications
* [elastic/timelion](https://github.com/elastic/timelion) time-series analyses application. Overview and installation guide: Timelion: [The time series composer for Kibana](https://www.elastic.co/blog/timelion-timeline)
* [Kibana Alert App for Elasticsearch](https://github.com/elasticfence/kaae) - Kibana plugin with monitoring, alerting and reporting capabilities

### Kibana Visualization plugins
* [nbs-system/mapster](https://github.com/nbs-system/mapster) - a visualization which allows to create live event 3d maps in Kibana
* [Kibana Tag Cloud Plugin](https://github.com/stormpython/tagcloud) - tag cloud visualization plugin based on d3-cloud plugin

## Discussions and social media
* [/r/elasticsearch](https://www.reddit.com/r/elasticsearch)
* [Elasticsearch forum](https://discuss.elastic.co/)
* [Stackoverflow](http://stackoverflow.com/tags/elasticsearch/hot)
* [Books on Amazon](http://www.amazon.com/s/ref=nb_sb_noss_1?url=search-alias%3Daps&field-keywords=elasticsearch) does not fit well into this category, but worth to check this out!
* TODO: Put some good twitter accounts

## Tutorials
* [Centralized Logging with Logstash and Kibana On Ubuntu 14.04](https://www.digitalocean.com/community/tutorial_series/centralized-logging-with-logstash-and-kibana-on-ubuntu-14-04) everything you need to now when you are creating your first Elasticsearch+Logstash+Kibana instance
* [dwyl/learn-elasticsearch](https://github.com/dwyl/learn-elasticsearch) a getting started tutorial with a pack of valuable references
* [Make Sense of your Logs: From Zero to Hero in less than an Hour! by Britta Weber](https://www.youtube.com/watch?v=8vgTBIoF8zs) demonstrates how you can build Elasticsearch + Logstash + Kibana stack to collect and discover your data

## Articles
## System configuration
* [A Useful Elasticsearch Cheat Sheet in Times of Trouble](http://logz.io/blog/elasticsearch-cheat-sheet/)
* [The definitive guide for Elasticsearch on Windows Azure](http://code972.com/blog/2014/07/74-the-definitive-guide-for-elasticsearch-on-windows-azure)
* [ElasticSearch pre-flight checklist](http://asquera.de/opensource/2012/11/25/elasticsearch-pre-flight-checklist/)
* [9 Tips on ElasticSearch Configuration for High Performance](https://www.loggly.com/blog/nine-tips-configuring-elasticsearch-for-high-performance/)
* [Docker and elasticsearch blog post series](http://blog.codingtimes.com/tag/elasticSearch/) by blog.codingtimes.com
* [Best Practices in AWS](https://www.elastic.co/guide/en/elasticsearch/plugins/master/cloud-aws-best-practices.html)
* [How to Secure Elasticsearch and Kibana](https://www.mapr.com/blog/how-secure-elasticsearch-and-kibana) with NGINX, LDAP and SSL :lock:

## Scalable Infrastructure and performance
* [Tuning data ingestion performance for Elasticsearch on Azure](https://azure.microsoft.com/en-us/documentation/articles/guidance-elasticsearch-tuning-data-ingestion-performance/) - and not only for Azure. That's a great article about Elasticsearch Performance testing by example
* [Elasticsearch Indexing Performance Cheatsheet](https://blog.codecentric.de/en/2014/05/elasticsearch-indexing-performance-cheatsheet/) - when you plan to index large amounts of data in Elasticsearch (by Patrick Peschlow)
* [ElasticSearch for Logging](http://edgeofsanity.net/article/2012/12/26/elasticsearch-for-logging.html) Elasticsearch configuration tips and tricks from Sanity
* [Scaling Elasticsearch to Hundreds of Developers](http://engineeringblog.yelp.com/2014/11/scaling-elasticsearch-to-hundreds-of-developers.html) by Joseph Lynch @yelp
* [10 Elasticsearch metrics to watch](http://radar.oreilly.com/2015/04/10-elasticsearch-metrics-to-watch.html)
* [Understanding ElasticSearch Performance](https://joshrendek.com/2015/11/understanding-elasticsearch-performance/)
* [Our Experience of Creating Large Scale Log Search System Using ElasticSearch](http://www.cubrid.org/blog/dev-platform/our-experience-creating-large-scale-log-search-system-using-elasticsearch/) - topology, separate master, data and search balancers nodes
* :open_file_folder: [Elasticsearch on Azure Guidance](https://github.com/Azure/azure-content/blob/master/articles/guidance/guidance-elasticsearch.md) it is 10% on Azure and 90% of a very valuable general information, tips and tricks about Elasticsearch
* [How to avoid the split-brain problem in Elasticsearch](http://blog.trifork.com/2013/10/24/how-to-avoid-the-split-brain-problem-in-elasticsearch/)

### Integrations
* [Apache Hive integration](https://www.elastic.co/guide/en/elasticsearch/hadoop/current/hive.html)
* [Connecting Tableau to ElasticSearch (READ: How to query ElasticSearch with Hive SQL and Hadoop)](http://ryrobes.com/systems/connecting-tableau-to-elasticsearch-read-how-to-query-elasticsearch-with-hive-sql-and-hadoop/)
* [mradamlacey/elasticsearch-tableau-connector](https://github.com/mradamlacey/elasticsearch-tableau-connector)

### Logging
* [5 Logstash Alternatives](https://sematext.com/blog/2016/09/13/logstash-alternatives/) and typical use cases

### Alerts
* [ElastAlert: Alerting At Scale With Elasticsearch, Part 1](http://engineeringblog.yelp.com/2015/10/elastalert-alerting-at-scale-with-elasticsearch.html) by engineeringblog.yelp.com
* [ElastAlert: Alerting At Scale With Elasticsearch, Part 2](http://engineeringblog.yelp.com/2016/03/elastalert-part-two.html) by engineeringblog.yelp.com
* [Elastalert: implementing rich monitoring with Elasticsearch](https://alexandreesl.com/2016/04/15/elastalert-implementing-rich-monitoring-with-elasticsearch/)

### Time series
* [Elasticsearch as a Time Series Data Store](https://www.elastic.co/blog/elasticsearch-as-a-time-series-data-store) by Felix Barnsteiner
* [Running derivatives on Voyager velocity data](https://www.elastic.co/blog/out-of-this-world-aggregations) By Colin Goodheart-Smithe
* Shewhart Control Charts via Moving Averages: [Part 1](https://www.elastic.co/blog/staying-in-control-with-moving-averages-part-1) - [Part 2](https://www.elastic.co/blog/staying-in-control-with-moving-averages-part-2) by Zachary Tong
* Implementing a Statistical Anomaly Detector: [Part 1](https://www.elastic.co/blog/implementing-a-statistical-anomaly-detector-part-1) - [Part 2](https://www.elastic.co/blog/implementing-a-statistical-anomaly-detector-part-2) - [Part 3](https://www.elastic.co/blog/implementing-a-statistical-anomaly-detector-part-3) by Zachary Tong

### Machine Learning
* [Classifying images into Elasticsearch with DeepDetect](http://www.deepdetect.com/tutorials/es-image-classifier/) ([forum thread with discussion](https://discuss.elastic.co/t/categorizing-images-with-deep-learning-into-elasticsearch/33217)) by Emmanuel Benazera
* [Elasticsearch with Machine Learning](https://medium.com/hello-elasticsearch/elasticsearch-amazon-machine-learning-7d7b979c328d#.s50a6d5mn) ([English translation](https://translate.googleusercontent.com/translate_c?depth=1&hl=en&prev=search&rurl=translate.google.com&sl=ja&u=https://medium.com/hello-elasticsearch/elasticsearch-amazon-machine-learning-7d7b979c328d&usg=ALkJrhioEPGsVRglGPFTa6w2ZfM-ydSoeg)) by Kunihiko Kido
* [Recommender System with Mahout and Elasticsearch](https://www.mapr.com/products/mapr-sandbox-hadoop/tutorials/recommender-tutorial)


### Use cases for elastic search
* [Data Infrastructure at IFTTT](http://engineering.ifttt.com/data/2015/10/14/data-infrastructure/) Elasticsearch, Kafka, Apache Spark, Redhsift, other AWS services
* [OFAC compliance with ElasticSearch](https://israelwebdev.wordpress.com/2015/01/19/ofac-compliance-with-elasticsearch/) using AWS
* [Building a Streaming Search Platform](https://blog.insightdatascience.com/building-a-streaming-search-platform-61a0d5a323a8#.f4b0rvae5) -
Streaming Search on Tweets: Storm, Elasticsearch, and Redis


## Other
* [LogZoom, a fast and lightweight substitute for Logstash](https://packetzoom.com/blog/logzoom-a-fast-and-lightweight-substitute-for-logstash.html)
* [Graylog2/graylog2-server](https://github.com/Graylog2/graylog2-server) - Free and open source log management (based on ES)
* [Fluentd vs. Logstash for OpenStack Log Management](http://www.slideshare.net/td-nttcom/fluentd-vs-logstash-for-openstack-log-management)
* [Building a Directory Map With ELK](http://david.pilato.fr/blog/2015/12/10/building-a-directory-map-with-elk/)
* [Structured logging with ELK - part 1](http://engineering.laterooms.com/structured-logging-with-elk-part-1/)
* [Search for :yum: Emoji with Elasticsearch :mag_right:](http://jolicode.com/blog/search-for-emoji-with-elasticsearch)
* [Complete Guide to the ELK Stack](http://logz.io/learn/complete-guide-elk-stack/)

## Videos
### Overviews
* [ElasticSearch in action Thijs Feryn](https://www.youtube.com/watch?v=oPObRc8tHgQ) a begginer overview
* [How we scaled Raygun](https://raygun.io/blog/2014/05/talk-how-we-scaled-raygun-using-technologies-like-elastic-search-featuring-iron-man/)
* [Getting started with ElasticSearch](https://www.youtube.com/watch?v=60UsHHsKyN4&list=PLw5h0DiJ-9PDStvJYc1LOZiEm1ehlEKLP)
* [Speed is a Key: Elasticsearch under the Hood](https://www.youtube.com/watch?v=vruklYSW4jg) introduction + basic performance optimization
* [$$ Pluralsight: Getting Started With Elasticsearch for .NET Developers](http://www.pluralsight.com/courses/elasticsearch-for-dotnet-developers) this course will introduce users to Elasticsearch, how it works, and how to use it with .NET projects.
* [$$ Complete Guide to Elasticsearch](https://www.udemy.com/elasticsearch-complete-guide/) Comprehensive guide to Elasticsearch, the popular search engine built on Apache Lucene
* [How Elasticsearch powers the Guardian's newsroom](http://www.infoq.com/presentations/elasticsearch-guardian)
* [Elasticsearch Query Editor in Grapfana](https://www.youtube.com/watch?v=hEztaMtobXw)  

### Advanced
* [#bbuzz 2015: Adrien Grand – Algorithms and data-structures that power Lucene and Elasticsearch](https://www.youtube.com/watch?v=eQ-rXP-D80U)
* [Rafał Kuć - Running High Performance Fault-tolerant Elasticsearch Clusters on Docker](https://www.youtube.com/watch?list=PLq-odUc2x7i_-qsarQo7MNsrYz3rlXGMu&v=D2zR-6Tke8o) and [slides](https://sematext.com/blog/2016/06/08/elasticsearch-in-docker/)

### Configuration file samples and other gists
* [ElasticSearch config for a write-heavy cluster](https://gist.github.com/reyjrar/4364063) - reyjrar/elasticsearch.yml

## Who is using elasticsearch?
[Yelp](http://engineeringblog.yelp.com/2015/10/how-we-use-deep-learning-to-classify-business-photos-at-yelp.html),
[IFTTT](http://engineering.ifttt.com/data/2015/10/14/data-infrastructure/),
[StackExchange](http://stackexchange.com/performance),
[Raygun](https://raygun.io/blog/2014/02/search-improvements-at-raygun/),
[Mozilla](https://www.youtube.com/watch?v=lWKEphKIG8U),
[Spotify](https://labs.spotify.com/2015/11/17/monitoring-at-spotify-introducing-heroic/),
[CERN](https://medium.com/@ghoranyi/needle-in-a-haystack-873c97a99983),
[NASA](https://www.elastic.co/elasticon/2015/sf/unlocking-interplanetary-datasets-with-real-time-search)

## I want more! (Elasticsearch related resources)
* [Technology Explained Blog](https://alexandreesl.com/)
* [EagerElk](http://blog.eagerelk.com/)
* [Tim Roes Blog](https://www.timroes.de/)

# Contributing
* Make sure you are about to post a valuable resource that belongs to this list
* Use spellchiker
* All spelling and grammar corrections are welcome
* Fork this repo, do your edits, send the pull request
* Feel free to create any new sections
* Add yourself to the "Contributors" section if you will
* Do not even try to add this repo to any awesome-awesome-* lists

# Contributors
@dzharii, @...

#### ← [Awesome TypeScript](https://github.com/dzharii/awesome-typescript) -= Awesome Elasticsearch =-
