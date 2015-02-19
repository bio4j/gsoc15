## Integrate Reactome data into Bio4j

- **difficulty** _medium_
- **technologies** _aws++, biology++, scala++, java++, git++_

Biological pathways data itself is extremely useful in life sciences basic research as well as in applied research in precision medicine or biotechnology. Graph database technologies enable the modeling of this kind of data in a way much closer to their natural structure.

[Reactome](http://www.reactome.org/) is a curated and manually reviewed database of biological pathways. It contains  pathways specifically designed for each species, with the _reaction_ being the basic unit. The pathways are defined as the set of biological entities such as proteins, nucleic acids or small molecules that are involved in a set of reactions from a particular biological network together with the relations among them. We will need to design a convenient graph model for all this, integrating not only the Reactome data but also all the existing links to other entities already in Bio4j (proteins, enzymes, GO terms, taxa, etc).

A biology/bioinformatics background would be almost necessary; you should be able to read biological texts and understand basic molecular biology concepts.

### Expected outcome

A/some bio4j module/s providing access to Reactome data linked with bio4j model entities. 

### Mentors

Some of the mentors that might be involved in the idea

- **[@epareja](https://github.com/epareja)** (<mailto:epareja@era7.com>)
    He's got a strong background in human biology and special interest in human signalling pathways.
- **[@rtobes](https://github.com/rtobes)** (<mailto:rtobes@era7.com>)
    She led and supervised the definition and implementation of the biological data model of the current Bio4j modules (UniProt, GO, EnzymeDB and NCBI taxonomy)
- **[@marina_manrique](https://github.com/rtobes)** (<mailto:mmanrique@era7.com>)
- **[@eparejatobes](https://github.com/eparejatobes)** (<mailto:eparejatobes@ohnosequences.com>)
    

If you are interested ask on the **[bio4j/gsoc15](https://gitter.im/bio4j/gsoc15?utm_source=share-link&utm_medium=link&utm_campaign=share-link)** gitter channel.
