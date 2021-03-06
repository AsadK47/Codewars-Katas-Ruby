# Task
You will be given an vector of string(s). You must sort it alphabetically (case-sensitive!!) and then return the first value.

The returned value must be a string, and have "***" between each of its letters.

You should not remove or add elements from/to the array.

# Solution
```ruby
def two_sort(s)
  s.min.chars.join("***")
end
```

# Explanation
1. What the code above is doing is using the .min function to get the values in the array by alphabetical order and reducing this value to 
the first value in the array. An alternative method to this would be to use .sort[0] which carrys out the same function, however, using
.min is significantly easier. 

2. The next step is splitting out the string into an array, so that each character is now seperated into it's own list or object
(the wording for this may not strictly true but you should test it to see what I mean!)

3. Finally we join the array back into a string, but not before putting *** between each value in that string.

Therefore an alternative solution to this example could be...solution 2!

# Solution 2
```ruby
def two_sort(s)
  s.sort[0].split('').join("***")
end
```

This may make more sense, using the explanation above, however, the first solution is generally easier and cleaner to execute!
