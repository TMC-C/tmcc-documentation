# Prerequisites

java 8, dotnet, maven, ??? (expand this)

# tmc-langs

## Setup

The C#-fork of tmc-langs can be cloned from https://github.com/TMC-C/tmc-langs.

Build the project with ```mvn clean package -DskipTests```. Tests are broken and skipped for now. Install the dependency to your local Maven repository with ```mvn clean install -U```.

## Running

The tmc-langs cli (command line interface) can be used to run tests for an exercise. 

Using the cli requires you have built the CSharp runner and have set the environment variable ```TMC_CSHARP_BOOTSTRAP_PATH``` (See the tmc-csharp-runner section below).

To run, use the command ```java -jar target\tmc-langs-cli-0.7.17-SNAPSHOT.jar run-tests --exercisePath [full path to exercise root folder] --outputPath testResults.txt```

This will run tests for the exercise and save the test results to the file ```testResults.txt```.

# tmc-csharp-runner 

## Setup

The runner can be cloned from https://github.com/TMC-C/tmc-csharp-runner.

Build the runner with ```dotnet build```.

Using the runner with tmc-langs requires you to set the full path to the compiled ```Bootstrap.dll``` file into the environment variable ```TMC_CSHARP_BOOTSTRAP_PATH```. The ```Bootstrap.dll``` file is contained in the folder ```[tmc langs root]/Bootstrap/bin/Debug/netcoreapp3.1/```. If on Windows, use double backslashes as folder separators in the path. For example ```C:\\whatever\\tmc-csharp-runner\\Bootstrap\\bin\\Debug\\netcoreapp3.1\\Bootstrap.dll```.

## Running

put stuff here
