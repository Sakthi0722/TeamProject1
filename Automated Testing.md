#Introduction to Automated Testing

Automation testing is a Software testing technique to test and compare the actual outcome with the expected outcome. This can be achieved by writing test scripts or using any automation testing tool. Test automation is used to automate repetitive tasks and other testing tasks which are difficult to perform manually. 

## Automated Testing Process

1. Test Tool Selection

2. Define scope of Automation

3. Planning, Design and Development

4. Test Execution

5. Maintenance

### Test tool selection
Test Tool selection largely depends on the technology the Application Under Test is built on. For instance, QTP does not support Informatica. So QTP cannot be used for testing Informatica applications. It's a good idea to conduct a Proof of Concept of Tool on AUT.

### Define the scope of Automation
The scope of automation is the area of your Application Under Test which will be automated. Following points help determine scope:

1. The features that are important for the business
2. Scenarios which have a large amount of data
3. Common functionalities across applications
4. Technical feasibility
5. The extent to which business components are reused
6. The complexity of test cases
7. Ability to use the same test cases for cross-browser testing

### Planning, Design, and Development
During this phase, you create an Automation strategy & plan, which contains the following details-

1. Automation tools selected
2. Framework design and its features
3. In-Scope and Out-of-scope items of automation
4. Automation testbed preparation
5. Schedule and Timeline of scripting and execution
6. Deliverables of Automation Testing

### Test Execution
Automation Scripts are executed during this phase. The scripts need input test data before there are set to run. Once executed they provide detailed test reports.

Execution can be performed using the automation tool directly or through the Test Management tool which will invoke the automation tool.

**Example**: Quality center is the Test Management tool which in turn it will invoke QTP for execution of automation scripts. Scripts can be executed in a single machine or a group of machines. The execution can be done during the night, to save time.

### Test Automation Maintenance Approach
Test Automation Maintenance Approach is an automation testing phase carried out to test whether the new functionalities added to the software are working fine or not. Maintenance in automation testing is executed when new automation scripts are added and need to be reviewed and maintained in order to improve the effectiveness of automation scripts with each successive release cycle.

### Types of Automated Testing
1. Smoke Testing
2. Unit Testing
3. Integration Testing
4. Functional Testing
5. Keyword Testing
6. Regression Testing
7. Data Driven Testing
8. Black Box Testing

### Automation Testing Tools
There are tons of Functional and Regression Testing Tools available in the market. Here are some best:

1. Ranorex Studio
2. Testim
3. 21
4. Selenium
5. QTP (MicroFocus UFT)
6. Rational Functional Tester
7. WATIR
8. SilkTest
