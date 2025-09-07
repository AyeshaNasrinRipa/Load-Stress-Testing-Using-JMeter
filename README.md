# Booking Performance Testing with JMeter

This repository contains a complete JMeter setup for testing the performance of the **Restful Booker API** using login, booking creation, and booking search scenarios. Both **load testing** and **stress testing** were performed, and reports are included.

---

## Contents
- `booking.jmx` — JMeter test plan (Login → Create Booking → Search Booking)
- `booking-api-test-report.xlsx` — Excel file with load test report and stress test execution steps and report

---

## Scenario
**120,000 users over a 12-hour period** log in, create a booking, and search for the booking.

- **Todo 1:** Perform load test in 3 steps (5 min, 10 min, 20 min) using Gaussian Random Timer (Deviation = 2000ms, Constant Delay = 500ms). Generate HTML report and Excel results.
- **Todo 2:** Conduct stress test by gradually increasing users until bottleneck throughput is found. Generate report.
- **Todo 3:** Generate HTML reports for both load test and stress test, and add results into `booking-api-test-report.xlsx`.

---

## Prerequisites
- Java 17 LTS+
- Apache JMeter 5.6.3 installed
- Git installed

---

## Running the Tests


## Reports

### Load Testing
<img width="1710" height="699" alt="Load Testing Report" src="https://github.com/user-attachments/assets/d2918f91-746e-42ee-9c1e-807885285d2c" />

### Stress Testing
<img width="1228" height="465" alt="Stress test Report" src="https://github.com/user-attachments/assets/8e07fff2-27bc-40a8-9348-68cd2ae09b3a" />

### Excel Test Report
- `booking-api-test-report.xlsx` contains 2 tabs:
  - **Load test report** with results from 5 min, 10 min, and 20 min runs
  - **Stress test report** with gradual user increases until bottleneck throughput was observed

---


