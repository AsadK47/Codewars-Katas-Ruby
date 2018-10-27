# Task
Given two numbers and an arithmetic operator (the name of it, as a string), return the result of the two numbers having 
that operator used on them.

a and b will both be positive integers, and a will always be the first number in the operation, and b always the second.

The four operators are "add", "subtract", "divide", "multiply".


# Solution
```ruby
def arithmetic(a, b, operator)
  case 
  when operator == "add"
  a + b
  when operator == "subtract"
  a - b
  when operator == "multiply"
  a * b
  when operator == "divide"
  a / b
 end
end
```
