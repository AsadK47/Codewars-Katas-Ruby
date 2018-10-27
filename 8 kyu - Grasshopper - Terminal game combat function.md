# Task
Create a combat function that takes the player's current health and the amount of damage recieved
and returns the player's new health. Health can't be less than 0.

# My solution
```ruby
def combat(health, damage)
  if health - damage > 0
    return health - damage
  else
    return 0
  end
end
```

# Factored solution
```ruby
def combat(health, damage)
  health - damage > 0 ? health - damage : 0
end
```

# Better Solution
```ruby
def combat(health, damage)
  [health-damage,0].max
end
```
