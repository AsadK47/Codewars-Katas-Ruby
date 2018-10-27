# Task
When provided with a number between 0-9, return it in words.

Input :: 1

Output :: "One".

Try using "Switch" statements.

# My solution
```ruby
def switch_it_up(number)
  case
  when number == 1
  return "One"
  when number == 2
  return "Two"
  when number == 3
  return "Three"
  when number == 4
  return "Four"
  when number == 5
  return "Five"
  when number == 6
  return "Six"
  when number == 7
  return "Seven"
  when number == 8
  return "Eight"
  when number == 9
  return "Nine"
 end
end
```

# Better / Factored Solution
```ruby
def switch_it_up(number)
  %w(Zero One Two Three Four Five Six Seven Eight Nine)[number]
end
```
