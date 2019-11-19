# Backend

The following software can be used as blocks to store and process the data on server. Some blocks may need to be integrated together, or missing features would need to be developed. Although most of those software can be configured or customised, the means to extend them are described in the [programming languages](/languages) section, and the means to bring them together into production are described in the [DevOps](/devops) section.

## Databases

### Relational databases

Relational databases allow a strict structuring of the data, that ensures its consistency, but comes at a cost: as the data structure is fixed, decentralisation of the data is only possible in defining strict sharding rules. When the database schema evolves, a strong data migration mechanism is required in order to ensure the relationships between data elements.

#### [PostgreSQL](https://www.postgresql.org/) <Badges user="postgres" repo="postgres" />

PostgreSQL is a powerful, open-source object-relational database system that uses and extends the SQL language combined with many features that safely store and scale the most complicated data workloads.

PostgreSQL has earned a strong reputation for its proven architecture, reliability, data integrity, robust feature set, extensibility, and the dedication of the open-source community behind the software to consistently deliver performant and innovative solutions. PostgreSQL runs on all major operating systems, is [ACID](https://en.wikipedia.org/wiki/ACID)-compliant, and has powerful add-ons such as the popular PostGIS geospatial database extender. PostgreSQL has become the open-source relational database of choice for many people and organisations.

#### [MySQL](https://www.mysql.com/) <Badges user="mysql" repo="mysql-server" />

MySQL is a relational database management system (RDBMS) developed by Oracle that is based on structured query language (SQL). MySQL is one of the world's most popular open-source database. With its performance, reliability and ease-of-use, MySQL has become a common choice for web-based applications. It's used by high profile web companies, such as Facebook, Twitter, YouTube, Yahoo! and more.

### NoSQL databases

NoSQL databases, or document databases, allow a more flexible data schema, and is easier to distribute. However the consistency of the data is often not guaranteed, and complex data schemas can become cumbersome to maintain, especially when it comes to its transformation for advanced analysis. NoSQL is often a good fit for loosely defined schemas, with little relationship between data elements.

#### [MongoDB](https://www.mongodb.com/) <Badges user="mongodb" repo="mongo" />

MongoDB is a general purpose, document-based, distributed database built for modern application developers and for the cloud era.

#### [CouchDB](http://couchdb.apache.org/) <Badges user="apache" repo="couchdb" />

Apache CouchDB is an open-source document-oriented NoSQL database, implemented in Erlang.

CouchDB uses multiple formats and protocols to store, transfer, and process its data, it uses JSON to store data, JavaScript as its query language using MapReduce, and HTTP for an API.

Unlike a relational database, a CouchDB database does not store data and relationships in tables. Instead, each database is a collection of independent documents. Each document maintains its own data and self-contained schema. An application may access multiple databases, such as one stored on a user's mobile phone and another on a server. Document metadata contains revision information, making it possible to merge any differences that may have occurred while the databases were disconnected.

## API

### [REST](https://en.wikipedia.org/wiki/Representational_state_transfer)

### [GraphQL](https://graphql.org/)

## Headless Content Management System

### [PostgREST](http://postgrest.org/) <Badges user="PostgREST" repo="postgrest" />

Using PostgREST is an alternative to manual [CRUD](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete) programming. Custom API servers suffer problems. Writing business logic often duplicates, ignores or hobbles database structure. Object-relational mapping is a leaky abstraction leading to slow imperative code. The PostgREST philosophy establishes a single declarative source of truth: the data itself.

### [Hasura GraphQL Engine](https://hasura.io/) <Badges user="hasura" repo="graphql-engine" />

Hasura GraphQL Engine is a fast GraphQL server that gives instant, realtime GraphQL APIs over Postgres, with webhook triggers on database events, and remote schemas for business logic.

Hasura helps to build GraphQL apps backed by Postgres or incrementally move to GraphQL for existing applications using Postgres.

### [Strapi](https://strapi.io/) <Badges user="strapi" repo="strapi" />

Strapi is a free and open source headless CMS. It works with SQL and NoSQL databases and is easily customisable with custom data schema, routes and plugins. It can run on any cloud solution as well as on a dedicated server. It exposes the data over a REST API or a GraphQL API (with still some limitations).

<!-- ## Authentication/Authorisation

### OAuth

### JWT

### OpenID -->

## Storage

### [Minio](https://min.io/) <Badges user="minio" repo="minio" />

Minio is a performant object storage system that is fully compatible with Amazon S3. If fully integrates with identity and access management systems, and offers numerous ways to trigger computations.

### [Samba](https://www.samba.org/) <Badges user="samba-team" repo="samba" />

Samba is the implementation of the Microsoft network file system for Linux machines. It enables the development of simple, robust file sharing systems that interacts with Windows end users.

## Caching

### [Memcached](https://memcached.org/) <Badges user="memcached" repo="memcached" />

### [Redis](https://redis.io/) <Badges user="antirez" repo="redis" />

## Search Engines

### [Lucene](https://lucene.apache.org/) <Badges user="apache" repo="lucene-solr" />

Apache Lucene is a high-performance, full-featured text search engine library written entirely in Java. It is a technology suitable for nearly any application that requires full-text search, especially cross-platform.

### [ElasticSearch](https://www.elastic.co/) <Badges user="elastic" repo="elasticsearch" />

Elasticsearch is a search engine based on the Lucene library. It provides a distributed, full-text search engine with an HTTP web interface and schema-free JSON documents. Parts of the software are licensed under various open-source licenses, while other parts fall under the proprietary Elastic License. According to the DB-Engines ranking, Elasticsearch is the most popular enterprise search engine followed by Apache Solr, also based on Lucene.

## Message Brokers

### [RabbitMQ](https://www.rabbitmq.com/) <Badges user="rabbitmq" repo="rabbitmq-server" />

RabbitMQ is an open-source message-broker software (sometimes called message-oriented middleware) that originally implemented the Advanced Message Queuing Protocol (AMQP) and has since been extended with a plug-in architecture to support Streaming Text Oriented Messaging Protocol (STOMP), Message Queuing Telemetry Transport (MQTT), and other protocols.

### [Kafka](https://kafka.apache.org/) <Badges user="apache" repo="kafka" />

Apache Kafka is part of the well known Hadoop Big Data ecosystem. It has been developed by LinkedIn and donated to the Apache Software Foundation. Kafka aims to provide a unified, high-throughput, low-latency platform for handling real-time data feeds. It is a software where queues can be defined, applications may connect to the queue and transfer a message onto it. Kafka can connect to external systems (for data import/export) via Kafka Connect and provides Kafka Streams, a Java stream processing library.

## SMS messages

Sending SMS will eventually occur on a non-free medium, so the following list does not only contain open-source solutions.

Two approaches can be considered to send and receive text messages:

- To use a GSM modem or a compatible phone that would be connected to a server on premise. This solution doesn't rely on any internet connectivity, and as a consequence can be deployed anywhere there is a GSM connectivity. However it requires an additional burden for maintaining the server and the modem/phone with an acceptable level of availability.
- To delegate the handling of SMS collection and distribution to a cloud communication as a service company. The total cost may be eventually low, and it is possible to secure the service with a Service Level Agreement. The service would however be managed by an external provider, and on the internet, which implies different data protection measures, as well as a reliable internet connectivity.

### GSM Modem

Several libraries are avaiable to connect a computer with a GSM mobile or any other GSM device. We selected the three most popular ones:

- [Kannel](https://www.kannel.org/) <Badges user="markjeee" repo="kannel"/>
- [Jasmin](https://www.jasminsms.com/) <Badges user="jookies" repo="jasmin"/>
- [PlaySMS](https://playsms.org/) <Badges user="antonraharja" repo="playSMS"/>

### Cloud services

Alternatively, it is possible to delegate the sending and receiving of SMS to a cloud platform through an HTTP API. As explain in the above, this approach is not open-source, but you may want to keep it simple in delegating SMS management to a third party. Here are two of the most popular SMS cloud services:

- [Twilio](https://www.twilio.com/)
- [Clickatell](https://www.clickatell.com/)

### [RapidSMS](https://www.rapidsms.org/) <Badges user="rapidsms" repo="rapidsms"/>

On top of sending/receiving SMS, RapidSMS offers a full framework to sort, filter and route text messages, and to build applications on top of it. It is written in Python and is using the Django framework.
