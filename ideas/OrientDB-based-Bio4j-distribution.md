## OrientDB based Bio4j distribution

- **difficulty** _medium_
- **technologies** _orientdb, java, scala, aws, s3, ec2_
- **one-sentence description** _make possible to use Bio4j with OrientDB as a backend_

[OrientDB](www.orientechnologies.com/orientdb/) is one of the few open source graph databases that supports [local indexes](https://github.com/orientechnologies/orientdb/issues/1895) and has a pretty comprehensive API for [graph schemas](http://www.orientechnologies.com/docs/last/orientdb.wiki/Schema.html). From the OrientDB point of view, Bio4j with its peculiar needs is certainly an interesting opportunity to showcase Orient database flexibility to accommodate wildly different scenarios.

All the Bio4j code is based on [bio4j/angulillos](https://github.com/bio4j/angulillos), which you can think of as a strongly typed version of Blueprints/tinkerpop. The first part of the project then will consist on developing **bio4j/angulillos-orientdb**, a working OrientDB-based implementation of the angulillos API. You can take a look at [bio4j/angulillos-titan](https://github.com/bio4j/angulillos-titan) for something equivalent done for [Titan](http://thinkaurelius.github.io/titan/).

Once this is done, you will need to work on implementing all the schema management and type definition / initialization of the Bio4j graph, using **bio4j/angulillos-orientdb**. Again, the titan Bio4j distribution is a good example as to what this would look like: [bio4j/bio4j-titan](https://bio4j.com/bio4j/bio4j-titan). 

As an extra bonus, and if you have enough Scala skills you could do the equivalent tasks for our Scala API.

### Expected outcome

A Bio4j distribution based in OrientDB, taking advantage of all its specific features.

### Possible mentors

- **[@pablopareja](https://github.com/pablopareja)** (<mailto:ppareja@ohnosequences.com>)
- **[@eparejatobes](https://github.com/eparejatobes)** (<mailto:eparejatobes@ohnosequences.com>)
- **[@laughedelic](https://github.com/laughedelic)** (<mailto:aalekhin@ohnosequences.com>)
- **[someone from OrientDB](???)** _not yet defined_

If you are interested ask on the **[bio4j/gsoc15](https://gitter.im/bio4j/gsoc15?utm_source=share-link&utm_medium=link&utm_campaign=share-link)** gitter channel, or to any of the possible mentors.
