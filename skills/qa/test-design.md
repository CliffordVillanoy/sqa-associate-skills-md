# Test Design (ISTQB CTFL)

## Overview

Test design is the process of creating test cases based on defined techniques to ensure adequate coverage of system functionality while optimizing effort. It focuses on identifying input conditions, expected outcomes, and potential defect areas.

---

## Objectives

* Maximize defect detection with minimal test cases
* Ensure coverage of valid, invalid, and edge scenarios
* Align test cases with requirements and acceptance criteria

---

## Black-Box Test Design Techniques

### 1. Equivalence Partitioning (EP)

Divides input data into partitions where test cases are expected to behave similarly.

#### Example:

Input field accepts values from 1 to 100

* Valid partition: 1–100
* Invalid partitions: <1, >100

Test values:

* 50 (valid)
* 0 (invalid)
* 101 (invalid)

---

### 2. Boundary Value Analysis (BVA)

Focuses on testing values at the boundaries of input ranges, where defects are most likely to occur.

#### Standard boundaries:

* min-1
* min
* max
* max+1

#### Example:

Range: 1–100

Test values:

* 0, 1, 100, 101

---

### 3. Decision Table Testing

Used when system behavior depends on combinations of conditions.

#### Example:

| Condition | Valid Login | Valid Password | Expected Result |
| --------- | ----------- | -------------- | --------------- |
| 1         | Yes         | Yes            | Access Granted  |
| 2         | Yes         | No             | Error           |
| 3         | No          | Yes            | Error           |
| 4         | No          | No             | Error           |

---

### 4. State Transition Testing

Used when the system behavior depends on previous states.

#### Example:

Login attempts:

* After 3 failed attempts → account is locked

---

## White-Box Techniques (Awareness)

### Statement Coverage

Ensures each statement in the code is executed at least once.

### Decision Coverage

Ensures each decision outcome (true/false) is tested.

---

## Experience-Based Techniques

### Error Guessing

Uses tester experience to identify likely defect areas.

Examples:

* Empty inputs
* Special characters
* Unexpected user behavior

---

### Exploratory Testing

Simultaneous learning, test design, and execution.

Approach:

* Define test charter
* Execute and explore system behavior

---

## Best Practices

* Maintain traceability to requirements
* Combine multiple techniques when necessary
* Prioritize high-risk areas
* Include both positive and negative scenarios
* Ensure test cases are clear and reproducible

---

## Common Pitfalls

* Missing edge cases
* Overlapping test coverage
* Lack of negative test scenarios
* Poorly defined expected results

---

## Summary

Effective test design ensures structured, efficient, and high-quality testing. Applying ISTQB techniques enables better defect detection and improves overall software quality.
