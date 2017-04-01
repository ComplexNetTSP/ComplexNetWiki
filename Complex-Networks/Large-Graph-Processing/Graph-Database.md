## [Neo4j](http://www.neotechnology.com/neo4j/)
  - [Introduction to Neo4j (slides)](http://fr.slideshare.net/sakrsherif/neo4j)
  - [Neo4j use cases (pdf)](http://fr.slideshare.net/emileifrem/an-intro-to-neo4j-and-some-use-cases-jfokus-2011)
  - [Cypher Tutorial](http://www.neo4j.org/learn/cypher)
     - [Cypher Video Tutorial](http://vimeo.com/50389825#)
     - [Cypher  Reference Card](http://www.neo4j.org/assets/download/Neo4j_CheatSheet_v3.pdf)
     - [Another Cypher Tutorial](http://fr.slideshare.net/jexp/geekout-publish)
  - [Max Demarzi Blog on Neo4j](http://maxdemarzi.com/)

## Tinkerpop stack 
- [Gremlin](https://github.com/tinkerpop/gremlin/wiki)
  - [Introduction to Gremlin](http://fr.slideshare.net/maxdemarzi/introduction-to-gremlin)
  - Groovy
     - [Tutorial Groovy Closures](http://groovy.codehaus.org/Tutorial+2+-+Code+as+data%2C+or+closures)
     - [Practically Groovy: Reaching for each](http://www.ibm.com/developerworks/java/library/j-pg04149/index.html)
     - [Scoping and the Semantics of "def"](http://groovy.codehaus.org/Scoping+and+the+Semantics+of+%22def%22)
- [Titan](http://thinkaurelius.github.com/titan/)
  - [Aurelius (company that provide Titan)](http://thinkaurelius.com/)
     - [Bog](http://thinkaurelius.com/blog/)
  - [Titan Introduction](http://fr.slideshare.net/slidarko/titan-the-rise-of-big-graph-data)
  - [Thunderdome Python bindings to Titan](https://github.com/StartTheShift/thunderdome)
- [Faunus](http://thinkaurelius.github.com/faunus/)
  - [Graph algorithms in MapReduce](https://www.google.fr/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&ved=0CDAQFjAA&url=http%3A%2F%2Fwww.umiacs.umd.edu%2F~jimmylin%2Fpublications%2FLin_Schatz_MLG2010.pdf&ei=msQaUa6rJ8yBhQe3toEY&usg=AFQjCNEWy0XFjOQHmzLjNC_Wec1f_NXjAA) 
- [Tinkerpop Book](http://www.tinkerpopbook.com/)

## Apache
  - [Accumulo](https://accumulo.apache.org/)
  - [Giraph](https://giraph.apache.org/)
  - [HBase](https://hbase.apache.org/)
  - Spark
       - [Graphx](https://amplab.cs.berkeley.edu/publication/graphx-grades/)

## Python Wrapper
- Python Wrapper for Neo4j
  - [Python-embedded (default library from Neo4j)](http://docs.neo4j.org/chunked/1.6/python-embedded-reference-core.html)
  - [Py2Neo](http://py2neo.org/)
      - [Introduction to Py2Neo](http://fr.slideshare.net/nigelsmall/introduction-to-py2neo)
      - [Documentation](http://packages.python.org/py2neo/)
      - [Tutorials](http://py2neo.org/tutorials/)
  - [Neo4j-rest-client](https://github.com/versae/neo4j-rest-client)
      - [Neo4j-rest-client’s documentation](https://neo4j-rest-client.readthedocs.org/en/latest/)
  - [Bulbflow](http://bulbflow.com/)
  - [Pyblueprints](https://github.com/escalant3/pyblueprints)

## Tools
- [Geoff](http://nigelsmall.com/geoff) (File format for graph description)
- [Gremlin](https://github.com/tinkerpop/gremlin/wiki) (Gremlin is a graph traversal language)
   - [Gremlin Tutorial](http://fr.slideshare.net/slidarko/gremlin-a-graphbased-programming-language-3876581)
- [Temporal Graph with Neo4j](https://github.com/ccattuto/neo4j-dynagraph/wiki/Representing-time-dependent-graphs-in-Neo4j)
    - [Sociopatterns](http://www.sociopatterns.org/)

## Blog
- [Marko Rodriguez Blog on Graph DB](http://markorodriguez.com/)
  - [Movie Recommender Engine Example](http://markorodriguez.com/2011/09/22/a-graph-based-movie-recommender-engine/)
- [Lab41](http://lab41.github.io/)

## Papers  
- [An NSA Big Graph experiment](http://www.pdl.cmu.edu/SDI/2013/slides/big_graph_nsa_rd_2013_56002v1.pdf)

***

## Howto gremlin
### Howto connected to Neo4j from gremlin shell

```
>$ gremlin

          \,,,/
          (o o)
 -----oOOo-(_)-oOOo-----
gremlin> g = new Neo4jGraph("/usr/local/Cellar/neo4j/community-1.7.2-unix/libexec/data/graph.db")
==>neo4jgraph[EmbeddedGraphDatabase [/usr/local/Cellar/neo4j/community-1.7.2-unix/libexec/data/graph.db]]
gremlin>
```

### Howto delete all the indexes in Neo4j

```
gremlin> neo4j = g.getRawGraph()
gremlin> manager = neo4j.index()
gremlin> manager.nodeIndexNames().each{ g.dropIndex( it ) }
gremlin> manager.relationshipIndexNames().each{  g.dropIndex( it )  }
```
##### Howto create an index

```
gremlin> g.createIndex("myIndex", Vertex.class)
gremlin> idx = g.idx("myIndex")
gremlin> vertices.each{ idx.put(key,value,it) }
....
gremlin> g.idx("myIndex")[[key:value]]
```

### Video

[![Alt text for your video](http://img.youtube.com/vi/bqvDSioHYq8/0.jpg)](http://www.youtube.com/watch?v=bqvDSioHYq8)

[![Alt text for your video](http://img.youtube.com/vi/ZkAYA4Kd8JE/0.jpg)](http://www.youtube.com/watch?v=ZkAYA4Kd8JE)

[![Alt text for your video](http://img.youtube.com/vi/nJEfq8qduKA/0.jpg)](http://www.youtube.com/watch?v=nJEfq8qduKA)