# Task
You will be given an array (a) and a value (x). All you need to do is check whether the provided array contains the value.

Array can contain numbers or strings. X can be either. Return true if the array contains the value, false if not.

# My solution
```ruby
def check(arr,element)
  arr.include? element
end
```

# Alternate solutions
```ruby
def check(arr,element)
  arr.any?(element)
end
```

```ruby
def check(arr,element)
  !!arr.index(element)
end
```
