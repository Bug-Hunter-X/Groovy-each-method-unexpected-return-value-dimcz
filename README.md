# Groovy each method unexpected return value
This example demonstrates an unexpected behavior of the each method in Groovy.  The `each` method iterates through a collection and applies a closure to each element, but it returns the original collection rather than a modified one. This can lead to errors if you expect the `each` method to modify the list in place.  The solution shows how to achieve the expected modification.

## Bug
The provided code snippet shows the unexpected return from Groovy's `each` method. It intends to double each element in the list, but it fails to do so and prints the original list.

## Solution
The solution uses the `collect` method which returns a new list containing the results of applying the closure to each element of the original list.