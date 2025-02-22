# Elixir Enum.each and List Modification Bug

This example demonstrates a common error in Elixir when attempting to modify a list while iterating over it using `Enum.each`.  The issue arises because `Enum.each` does not modify the list in place; it passes a copy to the function for each iteration. Attempting to remove elements within the `Enum.each` block won't affect the original list.

The solution shows how to use `Enum.filter` for a more idiomatic and correct approach to remove elements from a list based on a condition.
