# JavaScript Function: Unexpected NaN Handling

This repository demonstrates a common but subtle bug in JavaScript functions involving NaN (Not a Number) values.  The provided code snippet showcases the issue and offers a potential solution.

## Bug Description

The JavaScript function `foo` aims to add two numbers.  While it successfully handles `null` values by returning 0, it fails to address the case where one of the input values is `NaN`. This results in `NaN` being propagated through the addition operation, potentially leading to unexpected behavior in larger applications.

## Bug Solution

The solution addresses the `NaN` handling by using `isNaN` to check for `NaN` inputs and returning an alternative value or an error message for a better and predictable result.