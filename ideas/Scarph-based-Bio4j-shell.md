## Scarph based Bio4j shell

- **difficulty** _easy / medium_
- **skills** _good Scala knowledge is required_
- **one-sentence description** _an interactive shell (REPL) for constructing Bio4j queries using Scarph_

Scarph is a Scala library for declaring graph schema and constructing queries, that are checked to conform to this schema at compile-time. It is very important for Bio4j as a cloud-based data platform, to have a way for building queries which are known to be safe in advance. There is a Scarph-based [domain model definition for Bio4j](https://github.com/bio4j/scala-model). So using Scarph DSL one can write queries for Bio4j that are sensible from the point of view of its schema — just as you would do with the Bio4j Java API.

The goal of this project is to create an interactive shell for constructing Bio4j queries in Scarph DSL. It will provide users with a more convenient way of discovering Bio4j domain model and checking their queries correctness. As these queries are just Scala expressions, an obvious solution would be just tuning Scala REPL and adding some extra functionality. Another possible solution is embedding Scala compiler. Any other ideas are welcome.

The basic functionality for the shell is

- autocomple for the next step of a query
- sensible error reporting
- printing all statically known information about query


### Possible mentors

- **[@laughedelic](https://github.com/laughedelic)** (<mailto:aalekhin@ohnosequences.com>)
- **[@eparejatobes](https://github.com/eparejatobes)** (<mailto:eparejatobes@ohnosequences.com>)

If you are interested ask on the **[bio4j/gsoc15](https://gitter.im/bio4j/gsoc15?utm_source=share-link&utm_medium=link&utm_campaign=share-link)** gitter channel, or to any of the possible mentors.
