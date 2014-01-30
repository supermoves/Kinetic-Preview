Suggested Development Environments
==================================
* Latest version of Git for your OS: [http://git-scm.com/downloads](http://git-scm.com/downloads)

* JDK 1.7 or later: [http://www.oracle.com/technetwork/java/javase/downloads/index.html](http://www.oracle.com/technetwork/java/javase/downloads/index.html)

* Eclipse IDE For Java Developers. Version 4.2 (Juno) or later: [http://www.eclipse.org/downloads/](http://www.eclipse.org/downloads/)

* Maven 3.0.3 or later: [http://maven.apache.org/download.cgi](http://maven.apache.org/download.cgi)

* For Windows 7 system, install the system patch package for jni:
  32 bit: [http://www.microsoft.com/en-us/download/details.aspx?id=5555](http://www.microsoft.com/en-us/download/details.aspx?id=5555)
  64 bit: [http://www.microsoft.com/en-us/download/details.aspx?id=14632](http://www.microsoft.com/en-us/download/details.aspx?id=14632 )

Download Kinetic Simulator and Java API runtime libraries, Java API Javadoc, and Examples
==================================
1. Clone the code: `git clone https://github.com/Seagate/Kinetic-Preview.git`

Getting Started With Simulator
==================================
1. Run "mvn clean package"

2. Start with java command: 
       `java -jar ./target/kinetic-0.5.0.1-SNAPSHOT-jar-with-dependencies.jar`

3. Test drive examples at `<Kinetic-Folder>/src/test/java`

4. Browse API JavaDoc:

        <Kinetic-Folder>/doc/api-javadoc
        <Kinetic-Folder>/doc/example-javadoc
   
Admin Command Line Usage
==================================
1. Verify `<Kinetic-Folder>/target/kinetic-0.5.0.1-SNAPSHOT-jar-with-dependencies.jar` exists

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

The Python client is currently distributed as byte code.  You can install it
with setuptools or distribute.

    easy_install <Kinetic-Folder>/lib/kinetic-0.5.0.1dev-py2.7.egg

Once you have the Simulator running you can get started with the Python
Kinetic client.

    >>> from kinetic import Client
    >>> c = Client('localhost', 8123)
    >>> c.put('mykey', 'myvalue')
    <kinetic.common.Entry object at 0x273e9d0>
    >>> c.get('mykey').value
    'myvalue'

Documentation is built in to the python modules via docstrings, or you can try
out some basic functionality with `kcmd` the Kinetic python command line tool.

    $ kcmd --help
    usage: kcmd [-h] [-H HOSTNAME] [-P PORT] [-v]
                {put,get,delete,list,next,prev,getr,deleter} ...

    positional arguments:
      {put,get,delete,list,next,prev,getr,deleter}
        put                 store value at key
        get                 read value at key
        delete              remove a key
        list                list keys from start to end
        next                read value at next key
        prev                read value at prev key
        getr                get keys from start to end
        deleter             remove keys from start to end

    optional arguments:
      -h, --help            show this help message and exit
      -H HOSTNAME, --hostname HOSTNAME
      -P PORT, --port PORT
      -v, --verbose         output more info (can stack)


Preview OpenStack Swift on Kinetic 
=============================================

[https://github.com/swiftstack/kinetic-swift](https://github.com/swiftstack/kinetic-swift)


