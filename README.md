# Unintended Variable Shadowing in Ada

This repository demonstrates a subtle bug in Ada caused by unintended variable shadowing. The Ada code calculates the product of two integers but produces unexpected output due to a naming conflict.

## Bug Description

The `Multiply` function correctly calculates the product of two integers. However, in the `Main` procedure, the variables `A`, `B`, and `C` are initialized to 10. When calling the `Multiply` function, the result is expected to be 100. Due to shadowing, the variables inside the function are treated independently from the variables in `Main`, causing the output to be incorrect.

## Solution

The solution involves renaming the variables within the `Multiply` function to avoid the naming conflict. This ensures that the function uses the intended variables and produces the correct result.
