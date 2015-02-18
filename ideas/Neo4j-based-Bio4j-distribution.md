## Neo4j based Bio4j distribution

- **difficulty** _medium_
- **technologies** _aws, s3, ec2, neo4j, scala, java_
- **one-sentence description** _make possible to use Bio4j with Neo4j as a backend_

Neo4j is easily the most popular and widespread graph database engine, and there's a lot of interest in a Neo4j-based distribution of Bio4j.

All the Bio4j code is based on [bio4j/angulillos](https://github.com/bio4j/angulillos), which you can think of as a strongly typed version of Blueprints/tinkerpop. The first part of the project then will consist on developing [bio4j/angulillos-neo4j](https://github.com/angulillos-neo4j), targetting Neo4j 2.2; some preliminary work for this was done during the past few months. You can take a look at [bio4j/angulillos-titan](https://github.com/bio4j/angulillos-titan) for something equivalent done for [Titan](http://thinkaurelius.github.io/titan/).

Once this is done, you will need to work on implementing all the schema management and type definition/initialization of the Bio4j graph, using **bio4j/angulillos-neo4j**. Again, the titan Bio4j distribution is a good example as to what this would look like: [bio4j/bio4j-titan](https://bio4j.com/bio4j/bio4j-titan). 

As an extra bonus, and if you have enough Scala skills you could do the equivalent tasks for our Scala API.

### Expected outcome

A Bio4j distribution based in Neo4j, taking advantage of all its specific features.

### Mentors

- **[@pablopareja](https://github.com/pablopareja)** (<mailto:ppareja@ohnosequences.com>)
- **[@evdokim](https://github.com/evdokim)** (<mailto:ekovach@ohnosequences.com>)

If you are interested ask on the **[bio4j/gsoc15](https://gitter.im/bio4j/gsoc15?utm_source=share-link&utm_medium=link&utm_campaign=share-link)** gitter channel.