# Task
Very simple, given a number, find its opposite.

Examples:

1: -1
14: -14
-34: 34
But can you do it in 1 line of code and without any conditionals?

# My solution
```ruby
def opposite(n)
  if n
    return n*-1
  else
   return false
  end
end
```

# Better solution
```ruby
def opposite n
  -n
end
```
