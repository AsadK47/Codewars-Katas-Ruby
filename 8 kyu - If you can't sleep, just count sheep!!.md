# Task
If you can't sleep, just count sheep!!

Task:
Given a number, 3 for example, return a string with a murmur: "1 sheep...2 sheep...3 sheep..."

Note:
You will always receive a positive integer.

# Solution
```ruby
def count_sheep(num)
  (1..num).map {|i| "#{i} sheep..."}.join
end
```

# Explanation
The code returns from 1 to the designated number but iterates each time by interpolating the number to "sheep..." which is returned in 
an array and finally joined together to make it one long string.

This was difficult to describe, perhaps I don't know it well enough...
