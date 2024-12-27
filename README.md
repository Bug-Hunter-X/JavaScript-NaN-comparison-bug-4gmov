# JavaScript NaN Comparison Bug

This repository demonstrates a common, yet subtle, bug in JavaScript related to comparing NaN values.  The unexpected behavior of NaN with both loose and strict equality operators can lead to unexpected results in your code.

## Bug Description

In JavaScript, NaN (Not a Number) is a special value that represents an invalid numerical result.  The issue arises when attempting to compare two NaN values using either the loose equality operator (`==`) or the strict equality operator (`===`).  Both comparisons will incorrectly return `false`, even though the two values represent the same invalid numerical state.

## How to Reproduce

Clone this repository and run `bug.js`. You will see that the comparisons of NaN to itself using both loose and strict equality both evaluate to false.