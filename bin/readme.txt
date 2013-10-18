Kinetic Simulator/Admin Command Line Interface (CLI).

0. Assume you have at least Java SE 1.6 or later installed on your machine.
 
1. Define JAVA_HOME environment variable (example: google 'how to set JAVA_HOME on Mac).

2. Run "mvn clean package", verify <Kinetic-Folder>/target/kinetic-0.2.0.1-SNAPSHOT-jar-with-dependencies.jar exists.

3. To start Kinetic simulator:

   Windows: 
            cd <Kinetic-Folder>\bin
            startSimulator.bat
            
   Linux & Mac:
            cd <Kinetic-Folder>/bin
            sh startSimulator.sh
            
4. To run Kinetic admin CLI:

   Windows: 
            cd <Kinetic-Folder>\bin
            kineticAdmin.bat -help
            
   Linux & Mac:
            cd <Kinetic-Folder>/bin
            sh kineticAdmin.sh -help

5. Security file template: 
            security.template

6. To start Kinetic simulator (configuration port, tls_port and kinetic_home)

   Windows: 
            cd <Kinetic-Folder>\bin
            startSimulator.bat -help
            
   Linux & Mac:
            cd <Kinetic-Folder>/bin
            sh startSimulator.sh -help
   