# Boundary Value Analysis (BVA)

## Definition

Boundary Value Analysis is a black-box test design technique that focuses on testing values at the edges of input domains, where defects are most likely to occur.

---

## Objective

* Identify defects at boundary conditions
* Reduce number of test cases while maximizing effectiveness

---

## Standard Boundary Values

For a given range:

* Minimum - 1
* Minimum
* Maximum
* Maximum + 1

---

## Example

Input Range: 1–100

| Test Case | Value | Expected Result |
| --------- | ----- | --------------- |
| TC1       | 0     | Invalid         |
| TC2       | 1     | Valid           |
| TC3       | 100   | Valid           |
| TC4       | 101   | Invalid         |

---

## Types of Boundaries

* Numeric boundaries
* Length boundaries (e.g., password length)
* Date boundaries
* Range constraints

---

## Application Areas

* Form validation
* Input fields
* API parameter validation
* Financial and transactional systems

---

## Best Practices

* Always include both valid and invalid boundaries
* Combine with Equivalence Partitioning
* Validate system response, not just acceptance

---

## Common Mistakes

* Testing only valid boundaries
* Ignoring negative values
* Missing upper/lower edge cases

---

## Summary

Boundary Value Analysis is a highly effective technique for identifying defects at input limits and should be applied consistently in structured test design.
