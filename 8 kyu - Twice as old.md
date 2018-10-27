# Task
Your function takes two arguments:

current father's age (years)
current age of his son (years)
Сalculate how many years ago the father was twice as old as his son (or in how many years he will be twice as old).


### Solution ###
```ruby
def twice_as_old(dad, son)
    (dad - son * 2).abs
end
```

# Explanation
1. What this code is doing getting the dads age and minusing it from the sons. This means that regardless of how old the dad or the son
are, this, when multiplied by 2 will get the year of his father when he is twice as old as his son. 

2. The .abs function returns the absolute value of a number. This means that regardless of if the number is negative or postive, the 
return will always be a positive number
