## Integrate sequence data into Bio4j

- **difficulty** _medium_
- **technologies** _aws++, s3+++, dynamodb+++, biology+, scala++_

There is a lot of raw sequence data that is connected to the data already integrated in bio4j: Protein sequences, coding sequences (genes), RNA, etc. Some of this sequence data is available as part of Bio4j modules; however, graph databases are obviously not designed for storing (and indexing) essentially `String`s at this scale. Another key aspect here is that the needs of string matching in biology are pretty specific, depending on parameters such as 

- the type of sequences involved
- the subtle and complex issue of assigning biological meaning to sequence similarities
- the input for the queries

There is however a use case for which this integration would add great value: just being able to select a particular set of sequences based in the result of queries, which can take advantage of the rich model and integrated datasets; basically we are using the Bio4j graph as an index. For this the sequences could be stored as a combination of DynamoDB items and S3 objects, and then queries could return either just ids or the sequences themselves as needed.

In terms of implementing something giving the user the possibility of making queries about the sequence composition itself, we want to focus on **protein** sequences. Here just exact matches could be of use in some contexts, even more if it can be combined with graph traversals. The integration of domain specific tools such as `BLAST`-like local alignment tools would also be nice and incredibly useful.

### Expected outcome

A/some bio4j module/s providing access to sequence-based data linked with bio4j model entities. A more deep integration for **protein** sequences, allowing the user to query sequence composition, together with the integration of domain specific tools such as BLAST.

### Mentors

- **[@evdokim](https://github.com/evdokim)** (<mailto:ekovach@ohnosequences.com>)
    He's working right now on the development of cloud-based tools for metagenomics analysis using Bio4j, and on novel approaches to sequence indexing based on distributed weighted transducers.
- **[@eparejatobes](https://github.com/eparejatobes)** (<mailto:eparejatobes@ohnosequences.com>)
    He's supervising @evdokim's work on this.

If you are interested ask on the **[bio4j/gsoc15](https://gitter.im/bio4j/gsoc15?utm_source=share-link&utm_medium=link&utm_campaign=share-link)** gitter channel.