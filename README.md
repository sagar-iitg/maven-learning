```
<dependency>
    <groupId>jakarta.servlet</groupId>
    <artifactId>jakarta.servlet-api</artifactId>
    <version>6.0.0</version>
    <scope>provided</scope>

</dependency>

The provided dependencies are available only at compile time and in the test classpath of the project. These dependencies are also not transitive.

<dependency>
    <groupId>mysql</groupId>
    <artifactId>mysql-connector-java</artifactId>
    <version>8.0.28</version>
    <scope>runtime</scope>
</dependency>

The dependencies with this scope are required at runtime.
But we don’t need them for the compilation of the project code.
Because of that, dependencies marked with the runtime scope will be present in the runtime and test classpath,
but they will be missing from the compile classpath.

<dependency>
    <groupId>junit</groupId>
    <artifactId>junit</artifactId>
    <version>4.12</version>
    <scope>test</scope>
</dependency>

Test dependencies aren’t transitive and are only present for test and execution classpaths.


These are the maven classpaths mentioned below:

compile-classpath: Used at the time of compilation of application code.
 
test-classpath: Comes into use when testing the application code.
 
run-classpath: Used at the time of running or packaging of the application code.
In Maven, a dependency can either be direct or transitive.
Direct dependencies- These are defined explicitly in the POM file.
Transitive dependencies- The direct dependencies require these. These dependencies are automatically included in the Maven project’s classpath. Transitive dependencies are the dependencies of the dependencies which are included in the pom.xml file.



********* scope ********
compile  It is the default scope.
runtime
provided
test
system(deprecated) same sa provided 
import


The three build lifecycles are −

Clean: Cleans up artifacts created in previous builds.
 
Default: Used to create the application.
 
Site: Create a site document for your project.


There are three types of repositories:

Local repository
Remote repository
Central repository




```
