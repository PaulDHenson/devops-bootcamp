# Code Coverage:
Code coverage is the percentage of code which is covered by automated tests. Code coverage measurement simply determines which statements in a body of code have been executed through a test run, and which statements have not.

## Exercise:
You will be using Mocha and Istanbul to test the code coverage in the provided code. 

The following code is a series of functions written in javascript:

[sampleCode](https://raw.githubusercontent.com/PaulDHenson/devops-bootcamp/master/examples/codeQuality/javascript/simple.js ':include :type=code javascript')


The following code contains the unit tests that will be testing the javascript functions:

[testCode](https://raw.githubusercontent.com/PaulDHenson/devops-bootcamp/master/examples/codeQuality/javascript/simpleTest.js ':include :type=code javascript') 

Please perform the following:

    * Install Node
    * Install Mocha
    * Install Chai
    * Install Istanbul
    
    Note: When installing Chai and Istanbul with the npm command, use the -D tag to install as a developer dependency.

The provided javascript package.json file will have everything you need in order to pass the mocha tests; however, you will need to add to the file in order to get Istanbul to check your coverage.

[package](https://raw.githubusercontent.com/PaulDHenson/devops-bootcamp/master/examples/codeQuality/javascript/package.json ':include :type=code json')

Inside your package.json file under the “scripts” section, add a section called “coverage” and use the following command “nyc --reporter=text npm run test”
    
    Note: Make sure that your “test” section is running the following command “mocha ./simpleTest.js"