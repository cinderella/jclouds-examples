# Rackspace Examples
Example code that uses jclouds to perform common tasks on the Rackspace open cloud. The class names are self explanatory and the code is well commented for you to follow along.

## Requirements

1. Username and API key for the Rackspace open cloud - See the [Getting Started guide](http://www.jclouds.org/documentation/quickstart/rackspace/)
1. Java Development Kit (JDK) version 6 or later - [Download](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
2. Git - [Download](http://git-scm.com/downloads) or you can just [download this repository as a zip or tar.gz](https://github.com/jclouds/jclouds-examples/downloads)

## Environment
To setup an environment to compile and run the examples follow these instructions.

```
git clone https://github.com/jclouds/jclouds-examples.git
cd jcloud-examples/rackspace/
```
Now follow the instructions for [Getting the latest jclouds binaries](http://www.jclouds.org/documentation/userguide/installation-guide/). When you are done you should have a directory with the following files and sub-directories.

```
$ pwd
/Users/username/jclouds-examples/rackspace

$ ls
README.md    images/    lein    lib/    project.clj    src/
```
If you want to run the Logging example (which is strongly encouraged!) then you'll need the Logback JAR files. [Download](http://logback.qos.ch/download.html) the zip or tar.gz file, extract, and drop the JARs into the lib directory.

If you don't, you'll see this error when you try to run the Logging example but the example will still work.

```
SLF4J: Failed to load class "org.slf4j.impl.StaticLoggerBinder".
SLF4J: Defaulting to no-operation (NOP) logger implementation
SLF4J: See http://www.slf4j.org/codes.html#StaticLoggerBinder for further details.
```

## Command Line
To run these examples from the command line follow these instructions.

```
cd src/main/java/
javac -classpath ".:../../../lib/*:../resources/" org/jclouds/examples/rackspace/*.java

```
Every example class has a main method that takes your username as the first argument and your API key as the second argument. The one exception to this is the Authentication example that can take an optional third argument if you want to use your password for authentication.

Try out an example.

```
java -classpath ".:../../../lib/*:../resources/" org.jclouds.examples.rackspace.cloudservers.CreateServer myUsername myApiKey
```
Watch the terminal for output!

## Eclipse
To run these examples from Eclipse follow these instructions.

Create a new Java Project and choose jcloud-examples/rackspace/ as the Location.

![Eclipse: Create Java Project](https://raw.github.com/jclouds/jclouds-examples/master/rackspace/images/Eclipse1.png "Eclipse: Create Java Project")

This should create a project with the following Java Settings. Eclipse will have detected the lib directory and filled in all of the Libraries for you.

![Eclipse: Java Settings](https://raw.github.com/jclouds/jclouds-examples/master/rackspace/images/Eclipse2.png "Eclipse: Java Settings")

Try out an example.

1. Double click CreateContainer example file to open it
1. Choose the Run > Run Configurations... menu item
1. Press the plus icon to create a new launch configuration
1. This will automatically create a launch configuration for CreateContainer
1. Switch to the Arguments tab and enter your username and API key in the Program arguments field

![Eclipse: Launch Config](https://raw.github.com/jclouds/jclouds-examples/master/rackspace/images/Eclipse3.png "Eclipse: Launch Config")

Click Run and watch the Console for the output!

## Next Steps

Some suggestions.

1. Change the examples to do different things that you want to do
2. After running some examples, compare the output with what you see in the [Cloud Control Panel](https://mycloud.rackspace.com/)
3. Browse the [documentation](http://www.jclouds.org/documentation/)
3. Return to the [Installation Guide](http://www.jclouds.org/documentation/userguide/installation-guide/) and have a look at the different ways to integrate jclouds with your project
4. Join the [jclouds mailing list](https://groups.google.com/forum/?fromgroups#!forum/jclouds) or maybe even the [jclouds developer mailing list](https://groups.google.com/forum/?fromgroups#!forum/jclouds-dev)

Welcome to the jclouds [community](http://www.jclouds.org/documentation/community/)!