# Task
In this kata you will create a function that takes a list of 
non-negative integers and strings and returns a new list with the strings filtered out.

# Solution
```ruby
def filter_list(l)
  l.reject { |x| x.is_a? String }
end
```

# Different solution
```ruby
def filter_list(l)
  l.select{|i| i.is_a?(Integer)}
end
```
