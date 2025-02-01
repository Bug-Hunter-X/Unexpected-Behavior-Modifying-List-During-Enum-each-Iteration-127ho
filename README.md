# Elixir List Modification During Enum.each

This example demonstrates a common pitfall in Elixir when attempting to modify a list while iterating over it using `Enum.each`.  The issue arises because `Enum.each` doesn't modify the original list, and attempts to reassign `list` within the anonymous function only creates a new variable in that function's scope.