You don’t need to specify `int`, `string`, etc. Just assign a variable using numbers, boolean or `""`. (but you can using `Integer(gets.chomp)` for example!)

`my_num = 1` , `my_bool = true` , `my_string = "string"` 

`print` prints to the console, `puts` prints to the console with a new line.

There is a difference between `"` and `'`!
`"` allows string interpolation.

You can call methods on strings without it needing to be an assigned variable. 
e.g. `"this is a cool string".length` 

`.reverse` returns

You don’t always need brackets, although it still compiles with them. e.g.

```ruby
puts "name".upcase    # ==> NAME

puts("name".upcase)   # ==> NAME
```

Comments:

```ruby
# this is a single line comment

=begin
this is a multi-line comment
=end
```

`.capitalise` sets the first character to upper case and the rest to lower case.

Adding `!` to the end of a method call makes the variable equal the output. e.g.

`name.capitalize!` makes `name = name.capitalize` 

`gets` takes an input from the terminal.

`.chomp` removes new lines.

Instead of `if !this` Ruby uses `unless`

```ruby
unless hungry
	# do this if hungry is false (do this unless it is true)
else
  # do this if hungry is true
end
```

Lines that end with `?` result in booleans. e.g.

`if string.include? "character"` 

`gsub` substitutes a character.

Ruby has no `++`, use `+= 1` instead.

`for` loops in a range utilise `..` and `...`. `..` means between `x..y`, including y. `...` means between `x...y`, not including y.

```ruby
for num in 1..20
  puts num
end
# prints numbers 1 - 20, including 20.
```

To iterate through an object like an array, use `.each`.

Symbols are variables that are immutable and only exist in one place (one storage bit thing). Use them with `:`
`two:` is a symbol called two. They are often used for hash keys or referencing method names.

Use `.to_sym` / `.intern` and `.to_s` to swap them between strings and symbols.

![image.png](attachment:be868414-e93c-4b5c-866c-001181f95017:image.png)

From [this lesson](https://www.codecademy.com/courses/learn-ruby/lessons/a-night-at-the-movies/exercises/nice-work-1). CRUD!