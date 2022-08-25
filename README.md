# NoSQL Systems

## Learning Goals

- Gain understanding of different NoSQL types

## Introduction

Database systems traditionally were synonymous with Relational Database systems. Predominately over the last 10-15 year timeframe,
there has been a shift towards NoSQL systems being developed and utilized alongside or in place of Relational systems.
A driving factor in this have been attempts to solve the scaling problems we've seen in the previous sections, as well as rethinking data structures to be more optimized for given tasks.
In addition, the rise of DevOps practices and tooling has greatly reduced the initial up front cost of setting up and maintaining a new Database
environment. What traditionally would have required separate DBA specialists, and SysAdmins knowledgable in the intrinsicities of a novel
system, this can now be more easily deployed and managed.

The term 'NoSQL' doesn't really deliminate any specific given type of data store system or structure. It colloquially is understood to stand for "non-SQL", "not only SQL", and "non-relational".
Beyond these systems breaking away from using the traditional Relational data store type, there isn't necessarily much in common between
types of NoSQL systems. In fact, the development of a new system probably indicates there was a missing need with all of the previous
designs, leading to a good chance that each system is a complete new technology stack to understand and work with. This is unlike most Relational
systems that have been mostly standardized over the decades, and where skills from one vendor implementation are mostly transferable to
another.

## Different NoSQL Types

There are however general categories that most systems fall under.
Read through the following documentation for a good overview of this

- [Overview of NoSQL Types](https://redis.com/nosql/what-is-nosql/)

We will be experimenting with a few of the more commonly used systems in the next section

### Key Value

One of the most commonly used Key Value type NoSQL systems is Redis. It is commonly used for simple queuing systems, fast in-memory
caching, or any other situations where simple datatypes need to be stored in an independent server or service.

- [Overview of Redis](https://redis.io/docs/about/)

### Document

A very common Document type NoSQL system heavily used is Elasticsearch. Elasticsearch is commonly used in the logging aggregation space,
and text based search, where arbitrary fields and json fields may be ingested based on application specific needs and designs. Very fast text search
is a main design feature here.
		
- [Elasticsearch Intro](https://www.elastic.co/guide/en/elasticsearch/reference/8.3/elasticsearch-intro.html)
- [Elasticsearch Data Entry Overview](https://www.elastic.co/guide/en/elasticsearch/reference/8.3/documents-indices.html)
- [Elasticsearch Data Search Overview](https://www.elastic.co/guide/en/elasticsearch/reference/8.3/search-analyze.html)

### Graph

Graph Database systems tend to be delegated to more specific use cases. While you could feasibly use any of the other types in a general purpose way,
Graph based systems are really only useful for working with graphs with their objects and relations.

One of the more visible projects in this space would be Neo4j

- [Neo4j Introduction](https://neo4j.com/docs/getting-started/current/graph-database/)
		
        
### Column

Colume store NoSQL types best mimic the layout of what a traditional Database table looks like. However, actual usage and queries are
simplified compared to what Relational systems can do. Apache Cassandra is the system we will be covering in more depth.

Here is a quick overview.

- [Cassandra Overview](https://cassandra.apache.org/doc/latest/cassandra/architecture/overview.html)
