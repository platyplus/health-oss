# Backend

## Databases

### Relational databases

#### PostgreSQL <Badges user="postgres" repo="postgres" />

#### MySQL <Badges user="mysql" repo="mysql-server" />

### NoSQL databases

#### MongoDB <Badges user="mongodb" repo="mongo" />

#### CouchDB <Badges user="apache" repo="couchdb" />

## API

### REST

### GraphQL

## Caching

### Memcached <Badges user="memcached" repo="memcached" />

### Redis <Badges user="antirez" repo="redis" />

## Authentication/Authorisation

### OAuth

### JWT

### OpenID

## Message Brokers

### RabbitMQ <Badges user="rabbitmq" repo="rabbitmq-server" />

### Kafka <Badges user="apache" repo="kafka" />

## Search Engines

### Lucene <Badges user="apache" repo="lucene-solr" />

### ElasticSearch <Badges user="elastic" repo="elasticsearch" />

## Storage

### Minio <Badges user="minio" repo="minio" />

### Samba <Badges user="samba-team" repo="samba" />

## Headless CMS

### PostgREST <Badges user="PostgREST" repo="postgrest" />

### Hasura GraphQL Engine <Badges user="hasura" repo="graphql-engine" />

## SMS messages

Sending SMS will eventually occurr on a non-free medium, so the following list does not only contain open-source solutions.

Two approaches can be considered to send and receive text messages:

- To use a GSM modem or a compatible phone that would be connected to a server on premise. This solution doesn't rely on any internet connectivity, and as a consequence can be deployed anywhere there is a GSM connectivity. However it requires an additional burden for maintaining the server and the modem/phone with an acceptable level of availability.
- To delegate the handling of SMS collection and distribution to a cloud communication as a service company. The total cost may be eventually low, and it is possible to secure the service with a Service Level Agreement. The service would however be managed by an external provider, and on the internet, which implies different data protection measures, as well as a reliable internet connectivity.

### [RapidSMS](https://www.rapidsms.org/) <Badges user="rapidsms" repo="rapidsms"/>

On top of sending/receiving SMS, RapidSMS offers a full framework to sort, filter and route text messages, and to build applications on top of it. It is written in Python and is using the Django framework.

### GSM Modem

#### [Kannel](https://www.kannel.org/) <Badges user="markjeee" repo="kannel"/>

#### [Jasmin](https://www.jasminsms.com/) <Badges user="jookies" repo="jasmin"/>

#### [PlaySMS](https://playsms.org/) <Badges user="antonraharja" repo="playSMS"/>

### Cloud services

#### Twilio

#### Clickatell
