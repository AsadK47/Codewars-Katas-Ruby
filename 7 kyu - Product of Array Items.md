# Task
Calculate the product of all elements in an array.

If the array is nil or is empty, the function should return nil.

# My solution
```ruby
def product(arr)
  if arr.nil? 
    return nil
  else 
    arr.inject(:*)
  end
end
```

# Better solution
```ruby
def product(arr)
  arr&.reduce(:*)
end
```
