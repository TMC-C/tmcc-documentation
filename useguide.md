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

put stuff here

## Running

put stuff here
