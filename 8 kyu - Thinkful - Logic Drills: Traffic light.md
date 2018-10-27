# Task
You're writing code to control your town's traffic lights. 
You need a function to handle each change from green, to yellow, to red, and then to green again.

Complete the function that takes a string as an argument representing the current state of the light and 
returns a string representing the state the light should change to.

For example, update_light('green') should return 'yellow'.

# My solution
```ruby
def update_light(current)
  case
  when current == "green"
  return "yellow"
  when current == "yellow"
  return "red"
  when current == "red"
  return "green"
  end
end
```

# Better solution
```ruby
def update_light(current)
  {"green" => "yellow", "yellow" => "red", "red" => "green"}[current]
end
```

# Better solution 2
```ruby
def update_light(current)
  {
    'green' => 'yellow',
    'yellow'=> 'red',
    'red'   => 'green'
  }.fetch(current)
end
```

# Explanation
This an example of a case when statement. It just builds on when the light is X then change it to Y
