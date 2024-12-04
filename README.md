# Unexpected Behavior from Directly Modifying Instance Variables

This example demonstrates a potential issue in Ruby when directly modifying instance variables using `instance_variable_set`.  While it works, this practice is generally discouraged.

The example showcases a `MyClass` with a `value` method.  Direct manipulation of `@value` through `instance_variable_set` bypasses the intended method, potentially leading to inconsistencies and debugging challenges if not handled carefully.

**Recommended Approach:** Always use accessor methods to interact with instance variables for better code maintainability and predictability.