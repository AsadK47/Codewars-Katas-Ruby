# Task

# My solution
```ruby
def switcheroo(x) 
  x.tr("ab", "ba")
end
```

# Explanation
1. .tr replaces the strings a and b with their opposite b and a. You can also use gsub! in this situation but tr is easier for this one 

Use tr when you want to replace (translate) single characters.

tr matches on single characters (not via a regular expression), therefore the characters don't need to occur in the same order 
in the first string argument. When a character is found, it is replaced with the character that is found at the same index in the 
second string argument:

'abcde'.tr('bda', '123')
#=> "31c2e"

'abcde'.tr('bcd', '123')
#=> "a123e"
Use gsub when you need to use a regular expression or when you want to replace longer substrings:

'abcde'.gsub(/bda/, '123')
#=> "abcde"

'abcde'.gsub(/b.d/, '123')
#=> "a123e"
