# Task
Your task is to create a function that does four basic mathematical operations.

The function should take three arguments - operation(string/char), value1(number), value2(number).
The function should return result of numbers after applying the chosen operation.

# My solution
```ruby
def basic_op(operator, value1, value2)
  if operator == '+'
    return value1 + value2
  elsif operator == '-'
    return value1 - value2
  elsif operator == '*'
    return value1 * value2
  else operator == '/'
    return value1 / value2
 end
end
```

# Better solution
```ruby
def basic_op(operator, value1, value2)
  value1.send(operator, value2)
end
```

# Alternative solution
```ruby
def basic_op(o,a,b)
  eval [a,o,b].join
end
```
