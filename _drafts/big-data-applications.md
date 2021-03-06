---
layout: post
title: Big Data Stack
description: ""
tags: [startup, data]
share: true
---

# tl;dr

In the same way the open source [LAMP](http://en.wikipedia.org/wiki/LAMP_(software_bundle)) stack of Linux, Apache, MySQL and PHP, the big data stack has been established and will be the foundation of a next generation of applications.  Technology, previously only possible at Google, has been made accessible through the generation of this open source infrastructure.  This stack has accelerated the pace of innovation.

## Stack

This ecosystem is powered by service companies across the broader stack:
* AWS - cloud compute and storageHadoop, HDFS, HBase, MongoDB, Cassandra, Riak, Splunk, Amazon Redshift ... - data stores
* Scribe, Flume, Sqoop, Kafka - data ingestion
* Map Reduce, Hive, Pig, Cascading - batch data processing
* Spark, Impala, Drill, Presto, Tez / Stringer, Druid, Storm, S4 - real time data processing
* Lucene, SOLR, ElasticSearch - search
* Apache Mahout, Oryx / Myrrix, Kiji - modeling

## Infrastructure

Companies like Cloudera, Hortonworks, MapR[^1] and new comers like DataBricks, drive this big data stack innovation.  By offering, open source and licensed infrastructure, they enable big data.

## Application

**Manual**
With web click streams, mobile events, IoT sensors and more, data continues to grow [exponentially](http://techcrunch.com/2010/08/04/schmidt-data/).  The first order of business is to make it accessible and useful.  Actionable analytics is a first step, allowing for manual optimizations.

Analytics - databases and exploration
Business Intelligence - dashboards and visualization

As evidenced by companies creating actionable analysis of company data like Tableau, Datameer[^1], Looker[^1].

**Algorithmic**
The manual modeling and offline optimization gives way to algorithmic online models.

Relevance - ranking given a direct user intent (query)
Recommendation - given indirect user intent
Personalization - customization on a per user level
Anomaly Detection - fraud, threat
Forecast - model generation

Companies like Rich Relevance, WibiData, Sift Sciences, and Optimizely are providing recommendation, personalization and fraud detection as a service.

The result of which is the proliferation of tools and technology that is enabling big data applications previously only possible at places like Google.  These data scientists are creating the next generation of applications only now possible.

[^1]: Redpoint portfolio company.