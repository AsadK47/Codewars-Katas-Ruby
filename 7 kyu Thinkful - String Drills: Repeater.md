# Task
Write a class function named repeat() that takes two arguments (a string and a long integer), and returns a new string where the 
input string is repeated that many times. For example:

Repeater.repeat("a", 5)
should return

"aaaaa"

# My solution
```ruby
def repeater(string, n)
  string * n
end
```
