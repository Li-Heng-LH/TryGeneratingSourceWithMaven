# TryGeneratingSourceWithMaven


Walk through of tutorial of online course [Apache Maven: Beginner to Guru.](https://www.udemy.com/draft/2043700/?couponCode=GITHUB_REPO)

The purpose is to generate Java files from xsd. 

Run `mvn package`.

During build, jaxb2 plugin will run and execute _generate_ goal. 

Which will use xjc (XML Java Compiler) to generate Java files from xsd (XML Schema Definition). 