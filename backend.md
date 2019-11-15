# Backend

The following software can be used as blocks to store and process the data on server. Some blocks may need to be integrated together, or missing features would need to be developed. Although most of those software can be configured or customised, the means to extend them are described in the [programming languages](/languages) section, and the means to bring them together into production are described in the [DevOps](/devops) section.

## Databases

Two types of databases are commonly in use. Relational databases allow a strict structuring of the data, that ensures its consistency, but comes at a cost: as the data structure is fixed, decentralisation of the data is only possible in defining strict sharding rules. When the database schema evolves, a strong data migration mechanism is required in order to ensure the relationships between data elements.

On the other hand, NoSQL databases, or document databases, allow a more flexible data schema, and is easier to distribute. However the consistency of the data is often not guaranteed, and complex data schemas can become cumbersome to maintain, especially when it comes to its transformation for advanced analysis. NoSQL is often a good fit for loosely defined schemas, with little relationship between data elements.

### Relational databases

#### [PostgreSQL](https://www.postgresql.org/) <Badges user="postgres" repo="postgres" />

#### [MySQL](https://www.mysql.com/) <Badges user="mysql" repo="mysql-server" />

### NoSQL databases

#### [MongoDB](https://www.mongodb.com/) <Badges user="mongodb" repo="mongo" />

#### [CouchDB](http://couchdb.apache.org/) <Badges user="apache" repo="couchdb" />

## API

### [REST](https://en.wikipedia.org/wiki/Representational_state_transfer)

### [GraphQL](https://graphql.org/)

## Headless CMS

### [PostgREST](http://postgrest.org/) <Badges user="PostgREST" repo="postgrest" />

Using PostgREST is an alternative to manual [CRUD](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete) programming. Custom API servers suffer problems. Writing business logic often duplicates, ignores or hobbles database structure. Object-relational mapping is a leaky abstraction leading to slow imperative code. The PostgREST philosophy establishes a single declarative source of truth: the data itself.

### [Hasura GraphQL Engine](https://hasura.io/) <Badges user="hasura" repo="graphql-engine" />

### [Strapi](https://strapi.io/) <Badges user="strapi" repo="strapi" />

## SMS messages

Sending SMS will eventually occurr on a non-free medium, so the following list does not only contain open-source solutions.

Two approaches can be considered to send and receive text messages:

- To use a GSM modem or a compatible phone that would be connected to a server on premise. This solution doesn't rely on any internet connectivity, and as a consequence can be deployed anywhere there is a GSM connectivity. However it requires an additional burden for maintaining the server and the modem/phone with an acceptable level of availability.
- To delegate the handling of SMS collection and distribution to a cloud communication as a service company. The total cost may be eventually low, and it is possible to secure the service with a Service Level Agreement. The service would however be managed by an external provider, and on the internet, which implies different data protection measures, as well as a reliable internet connectivity.

## Authentication/Authorisation

### OAuth

### JWT

### OpenID

## Storage

### [Minio](https://min.io/) <Badges user="minio" repo="minio" />

### [Samba](https://www.samba.org/) <Badges user="samba-team" repo="samba" />

## Message Brokers

### [RabbitMQ](https://www.rabbitmq.com/) <Badges user="rabbitmq" repo="rabbitmq-server" />

### [Kafka](https://kafka.apache.org/) <Badges user="apache" repo="kafka" />

## Caching

### [Memcached](https://memcached.org/) <Badges user="memcached" repo="memcached" />

### [Redis](https://redis.io/) <Badges user="antirez" repo="redis" />

## Search Engines

### [Lucene](https://lucene.apache.org/) <Badges user="apache" repo="lucene-solr" />

### [ElasticSearch](https://www.elastic.co/) <Badges user="elastic" repo="elasticsearch" />

### [RapidSMS](https://www.rapidsms.org/) <Badges user="rapidsms" repo="rapidsms"/>

On top of sending/receiving SMS, RapidSMS offers a full framework to sort, filter and route text messages, and to build applications on top of it. It is written in Python and is using the Django framework.

### GSM Modem

#### [Kannel](https://www.kannel.org/) <Badges user="markjeee" repo="kannel"/>

#### [Jasmin](https://www.jasminsms.com/) <Badges user="jookies" repo="jasmin"/>

#### [PlaySMS](https://playsms.org/) <Badges user="antonraharja" repo="playSMS"/>

### Cloud services

#### Twilio

#### Clickatell
