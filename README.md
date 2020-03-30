# TryGeneratingSourceWithMaven


Walk through of tutorial of online course [Apache Maven: Beginner to Guru.](https://www.udemy.com/draft/2043700/?couponCode=GITHUB_REPO)


#### Generating Java files from xsd ####
The 1st task is to generate Java files from xsd. 

Run `mvn package`.

During build, jaxb2 plugin will run and execute _generate_ goal. 

Which will use xjc (XML Java Compiler) to generate Java files from xsd (XML Schema Definition).   

&nbsp;

**When is this plugin triggered?**   
* Before resources:resources goal. 
* If I override `<phase>` of plugin to `test`, it will execute during test phase, which means: 
* No classes will be generated in compile phase, as java files are not ready yet. 
* Java files will be generated in test phase. 


&nbsp;
#### Generating Java files from json schema #####
The 2nd task is to generate Java files from JSON Schema.  
commons-lang3 and jackson-databind are included as they are used in the generated pojo to compile into java class.   
If they are not included, compilation from generated pojo to java class will fail.  

Example project using the [jasonschema2pojo Maven Plugin](https://joelittlejohn.github.io/jsonschema2pojo/site/0.5.1/generate-mojo.html)

