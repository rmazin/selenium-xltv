# selenium-gradle
gradle build that executes selenium test

build / execute by running 
gradle test

Currently this script:

1. executes selenium
2. opens the Jenkins login page and does a string compare of an expected page title vs. actual
3. Opens XL Deploy to check if it's running
4. Opens XL Release and checks if it's running and can login with the provided credentials

The test as configured, should fail if any of the three programs are not running.

After execution, Junit XML output is located in build/test-results/TEST-myFirstTestngSelenium.MyFirstJunitClass.xml
