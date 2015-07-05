# Tutorial Jersey2 boiler plate code

# Maven
### Pre-requisites
* Java JDK 7
* Maven 3
* Eclipse Luna
* Jersey 2

### Create a maven application project
* using Command line:
```sh
mvn archetype:generate -DgroupId=com.techobyte -DartifactId=j2sample -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false
```
  IDE specific project file generation. Eclipse: ```mvn eclipse:eclipse``` IntelliJ: ```mvn idea:idea```
* using IDE: Eclipse/IntelliJ/Netbeans
  * New Maven Project
  * Archetype: maven-archetype-webapp
  * GroupId: com.techobyte
  * ArtifactId: j2sample

### Update Web Descriptor File (web.xml)
```xml
<web-app xmlns="http://java.sun.com/xml/ns/javaee"
   xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
   xsi:schemaLocation="http://java.sun.com/xml/ns/javaee 
   http://java.sun.com/xml/ns/javaee/web-app_3_0.xsd"
   version="3.0">
   <display-name>Servlet 3.0 Web Application</display-name>
</web-app>
```

### Add Dependency (pom.xml)
```xml
<project xmlns="http://maven.apache.org/POM/4.0.0"
   xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
   xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/maven-v4_0_0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <groupId>com.test</groupId>
   <artifactId>restex</artifactId>
   <packaging>war</packaging>
   <version>0.0.1</version>
   <name>j2sample Maven Webapp</name>
   <url>http://maven.apache.org</url>
   <dependencies>
      <dependency>
         <groupId>org.glassfish.jersey.containers</groupId>
         <artifactId>jersey-container-servlet</artifactId>
         <version>2.19</version>
      </dependency>
   </dependencies>
   <build>
      <finalName>j2sample</finalName>
   </build>
</project>
```

## Links
* [Java JDK 7]
* [Maven Plugins]
* [Jersey 2]

[Java JDK 7]:http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html
[Maven Plugins]:https://maven.apache.org/plugins/index.html
[Jersey 2]:https://jersey.java.net
