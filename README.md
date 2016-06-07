# Enumerator Coding Challenge

## Objectives

Become familiar with using common iterators introduced in the previous lesson.

???

### Code Challenge I: Using `.each`

Let's try out the enumerator methods we just learned. Refer back to the previous lesson to help you pass this challenge.

Below, we have a variable, `lunch_menu`, set equal to an array of lunch menu items.

Since you're super hungry and super excited about lunch, use the `.each` method to enumerate over the array and append an `"!"` ("exclamation mark") to each menu item. You can use the `<<` ("shovel operator") on each menu item string to add an `"!"` like this: `"pizza" << "!"`.

``` ruby
lunch_menu = ["pizza", "sandwich", "sushi", "soup", "salad"]
```

?: Which piece of code will achieve the desired result?

( )

``` ruby
lunch_menu << "!"
```

(x)

``` ruby
lunch_menu.each do |lunch_item|
  lunch_item << "!"
end
```

( )

``` ruby
lunch_menu.each do |lunch_item|
  "#{lunch_item}!"
end
```

( )

``` ruby
lunch_menu.each do |lunch_item|
```

### Code Challenge II: Using `.collect`

Below we have a variable, `nums`, set equal to an array of numbers. Enumerate over the array with the `.collect` method and return a new array of the squares of those numbers.

``` ruby
nums = [1, 2, 3, 4]
```

?: Which piece of code will achieve the desired result?

(x)

``` ruby
nums.collect { |n| n * n }
```

( )

``` ruby
nums.collect do |n|
  n + n
end
```

( )

``` ruby
nums.collect { |n| nn }
```

( )

``` ruby
nums.collect do |n|
  n
end
```

### Code Challenge III: Using `.select`

Below we have a variable, `odds_and_evens`, set equal to an array of numbers. Use the `.select` enumerator to iterate over the array and return any even numbers. This requires checking if a number is even. If you're unsure how to do that, reference the Ruby Documentation or try a google search!

``` ruby
odds_and_evens = [1, 3, 2, 18, 5, 10, 24]
```

?: Which piece of code will achieve the desired result?

( )

``` ruby
odds_and_evens.select do |n|
  n / 2
end
```

( )

``` ruby
odds_and_evens.select do |n|
  n % 2
end
```

(x)

``` ruby
odds_and_evens.select do |n|
  n.even?
end
```

( )

``` ruby
odds_and_evens.select do |n|
  n + 2
end
```

### Code Challenge IV: Using `.find`

Below we once again have a variable, `odds_and_evens`, set equal to an array of numbers. This time, use the `.find` method to iterate over the array and return only the *first* array element that is *odd*.

``` ruby
odds_and_evens = [2, 3, 2, 18, 5, 10, 24]
```

?: Which piece of code will achieve the desired result?

( )

``` ruby
odds_and_evens.find do |num|
  num.even?
end
```

( )

``` ruby
odds_and_evens.find do |num|
  num / 2
end
```

( )

``` ruby
odds_and_evens.find do |num|
  num
end
```

(x)

``` ruby
odds_and_evens.find do |num|
  num.odd?
end

```

### Code Challenge V: Using `delete_if`

Below we have a variable, `cats_and_dogs`, set equal to an array of strings that are either a `"cat"` or a  `"dog"`. We all know that cats and dogs don't get along. Iterate over the array and delete the elements that represent dogs.


``` ruby
cats_and_dogs = ["cat", "cat", "dog", "cat", "dog", "dog"]
```

?: Which piece of code will achieve the desired result?

(x)

``` ruby
cats_and_dogs.delete_if do |pet|
  pet == "dog"
end
```

( )

``` ruby
cats_and_dogs.delete_if do |pet|
  pet == "cat"
end
```

( )

``` ruby
cats_and_dogs.delete_if do |pet|
  pet == pet
end
```

( )

``` ruby
cats_and_dogs.delete_if do |pet|
  "dog"
end
```

### Code Challenge VI: Using `include?`

Below we have a variable, `famous_cats`, set equal to an array of famous cats. Use the `.include?` method to check and see if the array includes the string `"Maru"`.

``` ruby
famous_cats = ["Maru", "Lil Bub", "Grumpy Cat"]
```

?: Which piece of code will achieve the desired result?

(x)

``` ruby
famous_cats.include?("Maru")
```

( )

``` ruby
famous_cats.include?
```

( )

``` ruby
famous_cats.include?(true)
```

### Code Challenge VII: Using `any?`

Below we have a variable, `quiet_and_loud`, that is set equal to an array of strings. Use the `.any?` method to iterate over the array to determine if any of the words contained there are loud (upcased).

``` ruby
quiet_and_loud = ["hi", "HI", "shhh", "WHAT?!"]
```

?: Which piece of code will achieve the desired result?

( )

``` ruby
quiet_and_loud.any? { |w| w.upcase }
```

( )

``` ruby
quiet_and_loud.any? { w| w.upcase? }
```

(x)

``` ruby
quiet_and_loud.any? do |word|
  word == word.upcase
end
```

( )

``` ruby
quiet_and_loud.any? do |w|
  w
end
```

???

<p data-visibility='hidden'>View <a href='https://learn.co/lessons/enumerator-coding-challenge' title='Enumerator Coding Challenge'>Enumerator Coding Challenge</a> on Learn.co and start learning to code for free.</p>
