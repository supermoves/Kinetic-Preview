Suggested Development Environments
==================================
* Latest version of Git for your OS: [http://git-scm.com/downloads](http://git-scm.com/downloads)

* JDK 1.6 or later: [http://www.oracle.com/technetwork/java/javase/downloads/index.html](http://www.oracle.com/technetwork/java/javase/downloads/index.html)

* Eclipse IDE For Java Developers. Version 4.2 (Juno) or later: [http://www.eclipse.org/downloads/](http://www.eclipse.org/downloads/)

* Maven 3.0.3 or later: [http://maven.apache.org/download.cgi](http://maven.apache.org/download.cgi)

Download Kinetic Simulator and Java API runtime libraries, Java API Javadoc, and Examples
==================================
1. Clone the code: `git clone https://github.com/Seagate/Kinetic-Preview.git`

Getting Started With Simulator
==================================
1. Run "mvn clean package"

2. Start with java command: 
       `java -jar ./target/kinetic-0.2.0.1-SNAPSHOT-jar-with-dependencies.jar`

3. Test drive examples at `<Kinetic-Folder>/src/test/java`

4. Browse API JavaDoc:

        <Kinetic-Folder>/doc/api-javadoc
        <Kinetic-Folder>/doc/example-javadoc
   
Admin Command Line Usage
==================================
1. Verify `<Kinetic-Folder>/target/kinetic-0.2.0.1-SNAPSHOT-jar-with-dependencies.jar` exists

2. Define JAVA_HOME environment variable (example: google how to set JAVA_HOME on Mac).

3. To start Kinetic simulator:

   Windows: 
            cd <Kinetic-Folder>\bin
            startSimulator.bat
            
   Linux & Mac:
            cd <Kinetic-Folder>/bin
            sh startSimulator.sh
            
4. To run Kinetic admin Cli:

   Windows: 
            cd <Kinetic-Folder>\bin
            kineticAdmin.bat -help
            
   Linux & Mac:
            cd <Kinetic-Folder>/bin
            sh kineticAdmin.sh -help
            
Erlang client runtime library
==========================================
[https://github.com/basho-labs/riak_kinetic](https://github.com/basho-labs/riak_kinetic)

Python client runtime library
=============================================
       <Kinetic-Folder>/lib/kinetic-0.2.0.1dev-py2.7.egg
