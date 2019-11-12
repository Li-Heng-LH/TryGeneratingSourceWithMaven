# TryGeneratingSourceWithMaven


Walk through of tutorial of online course [Apache Maven: Beginner to Guru.](https://www.udemy.com/draft/2043700/?couponCode=GITHUB_REPO)


#### Generating Java files from xsd ####
The 1st task is to generate Java files from xsd. 

Run `mvn package`.

During build, jaxb2 plugin will run and execute _generate_ goal. 

Which will use xjc (XML Java Compiler) to generate Java files from xsd (XML Schema Definition). 


#### Generating Java files from json schema####
The 2nd task is to generate Java files from JSON Schema.

Example project using the [jasonschema2pojo Maven Plugin](https://joelittlejohn.github.io/jsonschema2pojo/site/0.5.1/generate-mojo.html)


