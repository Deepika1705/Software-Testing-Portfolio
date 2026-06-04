# Manual Testing Automation Testing and Performance Testing Assignment

## Candidate Name

DEEPIKA J

---

# Project Overview

This project covers:

* Manual testing
* Automation testing
* Performance testing using Apache JMeter
* Positive and negative test scenarios
* Test execution and reporting

Target API used for testing:

https://reqres.in/api/users?page=1

---

# Tools and Frameworks Used

| Tool / Technology     | Purpose                        |
| --------------------- | ------------------------------ |
| Apache JMeter         | Performance Testing            |
| Java                  | Automation Support             |
| Selenium WebDriver    | UI Automation                  |
| TestNG                | Test Execution Framework       |
| Excel                 | Manual Test Case Documentation |

---

# Tasks Completed

## Manual Testing

* Created detailed manual test cases for Claude.ai
* Covered both positive and negative scenarios
* Validated UI functionality and expected behavior

### Included Fields

* Test Case ID
* Test Scenario
* Preconditions
* Test Steps
* Expected Result
* Actual Result
* Status

---

## Automation Testing

Automation Testing – SauceDemo Website

Website Tested:

https://www.saucedemo.com/

## Tasks Completed

* Automated end-to-end testing for SauceDemo website using Selenium WebDriver and TestNG.
* Implemented login validation for valid and invalid credentials.
* Automated add-to-cart and remove-from-cart functionalities.
* Verified cart and checkout workflow.
* Performed UI validations for product details and buttons.
* Implemented Page Object Model (POM) framework design.
* Added reusable utility methods and screenshot capture on test failure.
* Generated execution reports using TestNG.


---

## Performance Testing

Performed load testing on the ReqRes API using Apache JMeter.

### Metrics Covered

* Average response time
* Minimum response time
* Maximum response time
* p90 / p95 response time
* Requests per second (Throughput)
* Failed requests
* Error rate (%)

---

# How to Run Automation Tests

## Prerequisites

Install the following:

* Java JDK 11 or above
* Eclipse IDE or IntelliJ IDEA
* Maven
* Apache JMeter

---

## Clone Repository

```bash
git clone <your-github-repository-url>
```

---

## Import Project

1. Open Eclipse
2. Click:
   File → Import → Existing Maven Project
3. Select the project folder
4. Click Finish

---

## Install Dependencies

Update Maven dependencies:

```bash
mvn clean install
```

---

## Run Automation Tests

Using TestNG:

1. Right click testng.xml
2. Select:
   Run As → TestNG Suite

OR using Maven:

```bash
mvn test
```

---

# How to Run Load Tests

## Install Apache JMeter

Download JMeter:

https://jmeter.apache.org/download_jmeter.cgi

Extract ZIP file and open:

```text
bin/jmeter.bat
```

---

## Configure API Request

### HTTP Request Settings

| Field       | Value      |
| ----------- | ---------- |
| Protocol    | https      |
| Server Name | reqres.in  |
| Method      | GET        |
| Path        | /api/users |

### Parameters

| Name | Value |
| ---- | ----- |
| page | 1     |

---

## Add HTTP Header Manager

Add header:

| Header Name  | Value            |
| ------------ | ---------------- |
| x-api-key    | YOUR_API_KEY     |
| Content-Type | application/json |

---

## Thread Group Configuration

| Setting         | Value      |
| --------------- | ---------- |
| Number of Users | 50         |
| Ramp-Up Period  | 10 seconds |
| Loop Count      | 5          |

---

## Add Listeners

* View Results Tree
* Summary Report
* Aggregate Report

---

## Execute Test

Click the Start button in JMeter to execute the performance test.

---

# Sample Performance Results

| Metric                | Value           |
| --------------------- | --------------- |
| Average Response Time | 320 ms          |
| Minimum Response Time | 110 ms          |
| Maximum Response Time | 2100 ms         |
| p95 Response Time     | 850 ms          |
| Throughput            | 18 requests/sec |
| Failed Requests       | 2               |
| Error Rate            | 0.8%            |

---

# Final Observation and Summary

The API handled concurrent requests successfully with acceptable response times and stable throughput.

Most requests were completed within the acceptable response time threshold, while the error percentage remained below 1%.

The performance test demonstrated that the API can handle moderate traffic efficiently without major failures.

---

# Any Assumptions or Issues Faced

## Assumptions

* Stable internet connection during execution
* Valid API key generated from ReqRes
* Java and JMeter installed correctly

---


