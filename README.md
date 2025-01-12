# CSS :nth-child Selector Bug

This repository demonstrates a common misunderstanding in using the `:nth-child` selector in CSS. The example shows how `:nth-child(n+1)` incorrectly selects all elements instead of only the first one.

## Bug

The provided CSS utilizes `:nth-child(n+1)` with the intention of selecting only the first element. However, this selector, due to the nature of `n` starting from 0, will select all elements.

## Solution

The solution replaces `:nth-child(n+1)` with `:nth-child(1)` to correctly select only the first element. For more complex patterns, ensure the formula in `:nth-child(an+b)` precisely targets the desired elements.