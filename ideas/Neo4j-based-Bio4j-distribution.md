## Neo4j based Bio4j distribution

- **difficulty** _medium_
- **technologies** _neo4j, java, aws, s3, ec2, scala_
- **one-sentence description** _make possible to use Bio4j with Neo4j as a backend_

[Neo4j](http://neo4j.com) is easily the most popular and widespread graph database engine, and there's a lot of interest in resurrecting a Neo4j-based distribution of Bio4j.

Starting from Bio4j 0.12, all the graph code is based on [bio4j/angulillos](https://github.com/bio4j/angulillos), which you can think of as a strongly typed version of Blueprints/tinkerpop. The first part of the project then will consist on developing an implementation of the angulillos API based on Neo4j: [bio4j/angulillos-neo4j](https://github.com/angulillos-neo4j), targetting Neo4j 2.2; some preliminary work for this was done during the past few months. You can also take a look at [bio4j/angulillos-titan](https://github.com/bio4j/angulillos-titan) for something equivalent done for [Titan](http://thinkaurelius.github.io/titan/).

Once this is done, you will need to work on implementing all the schema management and type definition/initialization of the Bio4j graph, using **bio4j/angulillos-neo4j**. Again, the titan Bio4j distribution is a good example as to what this would look like: [bio4j/bio4j-titan](https://bio4j.com/bio4j/bio4j-titan). 

As an extra bonus, and if you have enough Scala skills, you could do the equivalent tasks for our Scala API.

### Expected outcome

A Bio4j distribution based in Neo4j.

### Possible mentors

- **[@pablopareja](https://github.com/pablopareja)** (<mailto:ppareja@ohnosequences.com>)
- **[@evdokim](https://github.com/evdokim)** (<mailto:ekovach@ohnosequences.com>)
- **[@laughedelic](https://github.com/laughedelic)** (<mailto:aalekhin@ohnosequences.com>)

If you are interested ask on the **[bio4j/gsoc15](https://gitter.im/bio4j/gsoc15?utm_source=share-link&utm_medium=link&utm_campaign=share-link)** gitter channel.