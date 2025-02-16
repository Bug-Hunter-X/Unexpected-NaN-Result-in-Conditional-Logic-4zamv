# Unexpected NaN Result in Conditional Logic

This repository demonstrates an uncommon bug in JavaScript related to loose comparison and the handling of NaN (Not a Number) values in conditional logic.

## Description
The `foo` function aims to perform different operations based on the input `x`.  However, it doesn't explicitly check for NaN, leading to unexpected behavior when NaN is passed as an argument.  The loose comparison (`===`) is used, which should be more precise in this case.

## Bug
The bug lies in the lack of a check for NaN in the conditional logic. The function does not correctly handle the `NaN` input, resulting in NaN as output.