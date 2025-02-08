# Kotlin MutableList vs MutableMap removeIf() Behavior

This repository demonstrates a subtle difference in how `removeIf()` works with `MutableList` and `MutableMap` in Kotlin. The example highlights a potential source of unexpected behavior if not carefully considered.

## Bug

The `removeIf()` function operates differently on `MutableList` and `MutableMap` when used with a predicate that modifies the collection during the iteration.  This difference can lead to unexpected results.

## Solution

The solution focuses on using a safer approach that explicitly iterates and removes elements based on conditions, avoiding potential issues associated with concurrent modification.

## How to run

1. Clone the repository.
2. Open the project in your Kotlin IDE.
3. Run the main function in `bug.kt` and `bugSolution.kt` to see the different results.