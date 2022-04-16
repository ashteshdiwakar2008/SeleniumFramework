# SeleniumFramework
This framework is build with advance concepts of (Selenium, Java, Maven, TestNg, Extent Reports, Xcelite, Apache POI) to test web applications on multiple browsers with data driven capabilities and error free parallel execution

## Who can use it?
Anyone who wish to build a framework for Web UI Testing and plans to implement Test Driven Development (TDD) in the project.

## Why to use this framework design?
This framework is built using all the latest and most popular libraries and with a view to create a stable framework to automate Web UI applications so that Automation ROI is actually acheived. This project is built using best possible coding practices and following industry standards be it naming conventions or package definitions.

## Objectives or Principles implemented/followed: 
1. Single Responsibility Principle
2. Page Object Model Design Pattern
3. Factory Design
4. Singleton Design
5. Clean coding practices
6. Code reuse
7. Easy maintainability

## Package structure overview: 
1. src/main/java: 
    1. com.assertions : Contains a class where all common validation steps can be maintained which will be reflected in reports as well.
    2. com.constants : Contains a class which can be used to store framework level constant variables for referencing across various levels (viz, wait timeouts, etc).
    3. com.drivers : Contains classes to manage Web Driver instance and implementation for handling remote execution, parallel execution of tests for WebDriver reference.
    4. com.dataproviders : Contains class to mantain data provider for various tests.
    5. com.enums : Conatains various enums (For static value reference across project) based on requirements (viz. Browser Type, Wait type, etc.)
    6. com.pages : Contains class for each page on the web app and a Base Class for all page actions method references.
    7. com.listeners : Contains classes to provide definite implementation of TestNg listeners.
    8. com.reports : Contains class for custom Extent Report configurations.
    9. com.utilities : Contains calsses for various utility (viz. Reading Property Files data, Excel Utils, Screenshot Utils, etc.)
    
2. src/main/resources: 
    1. data : stores test data in excel sheets/json format
    2. config.properties : Contains project level configurations (viz. url, capture screenshot requests, browser details, etc.)
    
3. src/test/java: 
    1. com.hooks : Contains a class to manage application hooks i.e steps to be executed before scenario execution.
    2. com.runners : Contains class to manage test runners for various scenario based execution.
    3. com.stepdefinitions : Contains class to manage all steps as per page levels and feature file definitions.
    
## How to execute the tests
1. To execute the entire test suite --> use maven command mvn clean test
2. To execute individual test classes --> modify the testng.xml and execute as a suite file.

## To DO
[] Remote execution of test cases.
[] Capture screenshot for debugging purpose.
    
