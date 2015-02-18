## Angulillos and TinkerPop3

- **difficulty** _hard_
- **technologies** _java, TinkerPop3_
- **one-sentence description** _extend angulillos with a generic TinkerPop3 implementation_

[Angulillos](https://github.com/bio4j/angulillos) is a strongly-typed generic API for working with typed graphs, used extensively across Bio4j. Methods return Java 8 Streams of the corresponding edge/vertex types, and in/out methods can only be called if the target/source types of the correspoding types match.

[TinkerPop3](http://www.tinkerpop.com/docs/3.0.0.M7/) is a serious improvement over the previous releases, exposing a more functional programming oriented API centered around traversals; it is seriously lacking in terms of type safety though.

The idea is to develop an extension of the angulillos model which would be capable of expressing most of the TinkerPop3 traversal concepts in a type-safe way, and then develop an implementation of that API based on TinkerPop3.

This is a hard but really interesting project. If you are interested, ask @eparejatobes ASAP.

### Mentors

- **[@eparejatobes](https://github.com/eparejatobes)** (<mailto:eparejatobes@ohnosequences.com>)
- **[@laughedelic](https://github.com/laughedelic)** (<mailto:aalekhin@ohnosequences.com>)

If you are interested ask on the **[bio4j/gsoc15](https://gitter.im/bio4j/gsoc15?utm_source=share-link&utm_medium=link&utm_campaign=share-link)** gitter channel.


