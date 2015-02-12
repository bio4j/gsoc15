## AWS based Bio4j specific CI platform

- **difficulty** _hard_
- **technologies** _scala+++, sbt++, java, aws++++, s3, ec2, git_

Bio4j has really specific needs with respect to **continuous integration** and the release process in general. First, data and code releases need to be coordinated, as the data sources which we are integrating maintain their own version track while our API for them could be maintained independently. Other important point to consider is that testing involves the deployment of other components and resources in AWS; one needs to be sure that the import process went ok, that deploying the corresponding module is going to work across different AWS regions, etc.

As all of our release process is based around [sbt](https://github.com/sbt/sbt), we can take advantage of the good extension facilities available in the form of plugins. All coding will be done in Scala, experience with (or a strong desire towards rapidly acquiring it) type-level programming à la [shapeless](https://github.com/milessabin/shapeless) being a good asset here: the current strategy for dealing with all the different bio4j components being based on [Statika](https://github.com/ohnosequences/statika). 

Interacting with Amazon Web Services (mainly S3 and EC2) will be a critical part as all of our default bio4j stack is based on it. A basic understanding of git is a requirement, while knowledge and/or experience with TDD (test driven development) is a plus. We will try to build on top of existing CI platforms like Jenkins (for which there is at least a [sbt plugin](https://github.com/jenkinsci/sbt-plugin)) whenever possible, but the special requirements of bio4j could make this unreasonably hard; thus one of the first steps will be to evaluate whether this is an option.

### Expected outcome

A full-fledged CI solution for bio4j taking into account all the specifics of the bio4j platform.

### Mentors

- **[@laughedelic](https://github.com/laughedelic)** (<mailto:aalekhin@ohnosequences.com>)  
  The past few months he has been working developing sbt plugins for automating release proceses and interacting with AWS, and he is the main developer of [Statika](https://github.com/ohnosequences/statika).

- **[@eparejatobes](https://github.com/eparejatobes)** (<mailto:eparejatobes@ohnosequences.com>)  
  He's been designing and coordinating @laughedelic's work on Statika and sbt.

This idea is from [GSoC-2014](https://github.com/bio4j/gsoc14/wiki/AWS-based-bio4j-specific-CI-platform).
