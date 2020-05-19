# Prerequisites

Using tmc-langs and the tmc-csharp-runner requires you have installed the following:
- a Java 8 or higher [JDK](https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html) 
- a version of [Maven](https://maven.apache.org/download.cgi)
- [.NET](https://dotnet.microsoft.com/download) 3.1 or higher

# tmc-langs

## Setup

The C#-fork of tmc-langs can be cloned from https://github.com/TMC-C/tmc-langs.

Build the project with ```mvn clean package -DskipTests``` in the tmc-langs root folder. Tests are broken and skipped for now. Install the dependency to your local Maven repository with ```mvn clean install -U```.

## Running

The tmc-langs cli (command line interface) can be used to run tests for an exercise. 

Using the cli requires you have built the CSharp runner and have set the environment variable ```TMC_CSHARP_BOOTSTRAP_PATH``` (See the tmc-csharp-runner section below).

To run, use the command ```java -jar target\tmc-langs-cli-0.7.17-SNAPSHOT.jar run-tests --exercisePath [full path to exercise root folder] --outputPath testResults.txt``` in the root folder.

This will run tests for the exercise and save the test results to the file ```testResults.txt```.

# tmc-csharp-runner 

## Setup

The runner can be cloned from https://github.com/TMC-C/tmc-csharp-runner.

Build the runner with ```dotnet build``` in the runner root folder.

Using the runner with tmc-langs requires you to set the full path to the compiled ```Bootstrap.dll``` file into the environment variable ```TMC_CSHARP_BOOTSTRAP_PATH```. The ```Bootstrap.dll``` file is contained in the folder ```[tmc runner root]/Bootstrap/bin/Debug/netcoreapp3.1/```. If on Windows, use double backslashes as folder separators in the path. For example ```C:\\whatever\\tmc-csharp-runner\\Bootstrap\\bin\\Debug\\netcoreapp3.1\\Bootstrap.dll```.

## Running

put stuff here
