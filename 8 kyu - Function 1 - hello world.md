# Task
Description:
Make a simple function called greet that returns the most-famous "hello world!".

Style Points
Sure, this is about as easy as it gets. But how clever can you be to create the most creative hello world you can think of? 
What is a "hello world" solution you would want to show your friends?

# My solution
```ruby
def greet
  "hello world!"
end
```

# Better solution
```ruby
def greet
  "d0l1r2o3w45 67o8l9l10e11h".split(//).reverse.reject {|c| c.match(/\d/) }.join("") + "!"
end
```

# Best solution in my opinion
```ruby
eval 'def greet; ' + %~
 ________________________________________
/           'hello world!'               \
\                                        /
 ----------------------------------------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
~[55..68] + ' ;end'
```
