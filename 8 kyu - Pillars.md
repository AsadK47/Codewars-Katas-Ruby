There are pillars near the road. The distance between the pillars is the same and the width of the pillars is the same. 
Your function accepts three arguments:

number of pillars (≥ 1);
distance between pillars (10 - 30 meters);
width of the column (10 - 50 centimeters).
Calculate the distance between the first and the last pillar in centimeters (without the width of the first and last pillar).

# My solution
```ruby
def pillars(num_of_pillars, distance, width)
  if num_of_pillars == 1
    return 0
  elsif num_of_pillars == 2
    return ((num_of_pillars - 1) * distance) * 100
  else num_of_pillars >= 3
    return (((num_of_pillars - 1) * distance) * 100) + ((num_of_pillars - 2) * width)
  end
end
```

# Better (factored) solution
```ruby
def pillars(n, distance, width)
  [0, (n - 1) * (distance * 100 + width) - width].max
end
```
