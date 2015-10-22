This is one of the most simple Spark Scala projects you could imagine, packaged in one place for you to start working with Spark Scala.

# Building

To build this you will need a recent version of Scala and SBT installed.

SBT has packages for both Redhat and Debian available from http://www.scala-sbt.org/download.html

Scala has packages for Windows, Redhat and Debian available from http://www.scala-lang.org/download (pick a specific version to get links to vendor-specific packages)

With those installed, you can now run `sbt package` from the root of this repo and you'll get `target/scala-2.10/simple-project_2.10-1.0.jar` built.  Use this when running the apps listed below.

## SimpleApp

Usage: spark-submit --class SimpleApp simple-project.jar fileURL

One of the most simple Spark Scala apps you could imagine, printing out the number of lines with the letter A in and the number of lines with the letter B in.

## SimpleStreamingApp

Usage: spark-submit --class SimpleStreamingApp simple-project.jar

One of the most simple Spark Streaming Scala apps you could imagine, connecting to localhost:9999 and printing out a few word counts each second