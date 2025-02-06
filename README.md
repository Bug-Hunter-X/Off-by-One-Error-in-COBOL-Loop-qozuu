# COBOL Off-by-One Error

This repository demonstrates a common off-by-one error in COBOL loops. The provided COBOL code contains a `PERFORM VARYING` loop that incorrectly calculates the final value of a counter. The `bug.cob` file shows the erroneous code, while `bugSolution.cob` demonstrates the corrected version.

## Bug Description

The `PERFORM VARYING` loop intends to iterate 10 times, but due to an incorrect loop condition, it iterates 11 times. This is a classic off-by-one error, a frequent issue in programming. The root cause is the inclusive nature of the loop's `UNTIL` condition.