# Ruby Bug: Unexpected Behavior from Directly Modifying Instance Variables

This repository demonstrates a common, yet subtle bug in Ruby stemming from directly manipulating instance variables using `instance_variable_set` or similar methods. Directly accessing instance variables bypasses any methods designed to validate, control, or modify object state. This can lead to unexpected behavior, data inconsistency, and difficulty maintaining the code.  The solution shows proper accessor methods to prevent this issue.

## Bug Description:
The `bug.rb` file showcases how directly modifying an instance variable (`@value`) leads to correct output, but it undermines the intention of encapsulating data within the object.

## Solution:
The `bugSolution.rb` demonstrates a more robust approach where changes to the `@value` are managed through a method, ensuring encapsulation and data consistency.