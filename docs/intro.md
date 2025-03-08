---
sidebar_position: 1
---

# Introduction
Metatester is a framework that verifies the reliability, efficiency and coverage of automated tests.

It is currently in development stage.

# Problem
When developing automated testing, the usual focus is on the number and speed of tests, but a lot less focus on attempting to prove their reliability and effectiveness.

This can lead to a false sense of security and blind trust in the test results, without questioning the output.

When all tests have passed, some people wrongly assume that there are no issues.

Automated tests are proving that, for, and only for the cases declared in the tests, the system is functioninig correctly.

But if we are writing a program to verify another program, what makes us trust the code our test program is running?

# Solution
Automated verification and analysis of the test systems.

This is performed by simulating various types of defects, and run the tests against them.

# Isn't this mutation testing?
It might look similar to mutation testing, but it's not the same. 

Mutation testing is designed for unit tests, and it modifies the system code. Metatester does not modify the system code, it just simulates new behaviour.

# What types of testing can it verify?
REST API tests, with plans to extend to other layers like data, infrastructure, UI.

# What programming languages does it support?
Java, and also Python and Typescript in the future.

# Limitations
It supports tests written with RestAssured, but will be extended to other clients as well.

While Metatester can verify if the tests would catch more generic issues, it does not verify the specification coverage and effectiveness of the chosen test cases agains the specifications.