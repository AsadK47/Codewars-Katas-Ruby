# Task
Description:
Replace all vowel to exclamation mark in the sentence. aeiouAEIOU is vowel.

Examples
replace("Hi!") === "H!!"
replace("!Hi! Hi!") === "!H!! H!!"
replace("aeiou") === "!!!!!"
replace("ABCDE") === "!BCD!"

# My solution
```ruby
def replace(s)
  s.tr("aeiouAEIOU", "!")
end
```

# Alternate solution
```ruby
def replace(s)
  s.gsub(/([aeiou])/i, '!') 
end
```
