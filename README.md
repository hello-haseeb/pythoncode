


Project Title
A brief description of the project and what it does.

Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

Prerequisites
What things you need to install the software and how to install them:

Copy code
pip install -r requirements.txt
Running the code
To start the application, run:

Copy code
python swapiDevApplication.py
To run the performance tests, navigate to the performanceSuite/jmeter/bin directory and run:

Copy code
jmeter -n -t "../../perfTest.jmx" -l "../../output.jtl"
This will generate an output file output.jtl. To generate a report in csv format, navigate to performanceSuite/jmeter/lib/ext and run:

Copy code
java -jar CMDRunner.jar --tool Reporter --generate-csv "../../../aggregateReport.csv" --input-jtl "../../../output.jtl" --plugin-type AggregateReport
Finally, navigate back to the root directory and run the following command to analyze the results of the test:

Copy code
python -u performanceTestSuite.py
Press any key to terminate the server when you are done.

Authors
Your Name - Initial work - Your GitHub
License
This project is licensed under the MIT License - see the LICENSE.md file for details.

Acknowledgments
Hat tip to anyone whose code was used
Inspiration
etc

# PythonAssignment
This repo contains the python assignment. 

## Tools and frameworks used are as below:
- Python Flask - for web development
- RobotFramework - functional automation testing of api
- JMeter - for performance test

## Installation Required
- Java 11
- Python 3.11
- Pip

## Running the project
Compaitable for windows
There are 2 batch files:
- startAppAndRunRobotTests
  * To deploy server, install requirements and run functional automation tests using robotframework
- startAppAndPerformanceTest
  * To deploy server, install requirements and run performance test
