# Enumerator Coding Challenge

## Objectives

Become familiar using common iterators introduced in the previous lesson.


%%%

### Code Challenge I: Using `.each`

Let's try out the enumerator methods we just learned. Refer back to the previous lesson to help you pass this challenge.


Below, we have a variable, `lunch_menu`, set equal to an array of lunch menu items.

Since you're super hungry and super excited about lunch, use the `.each` method to enumerate over the array and append a "!" to each menu item. You can use the `<<` on each menu item string to add an "!". Like this: "pizza" << "!"

~~~ruby

lunch_menu = ["pizza", "sandwich", "sushi", "soup", "salad"]

#code your solution using .each here

~~~solution

lunch_menu.each do |lunch_item|
	lunch_item << "!""
end

~~~validation

assert_match(response, ["pizza!", "sandwich!", "sushi!", "soup!", "salad!"])

~~~

%%%

%%%

### Code Challenge II: Using `.collect`

Below we have a variable, `nums`, set equal to an array of numbers. Enumerate over the array with the `.collect` method and return a new array of the same numbers, squared.

~~~ruby

nums = [1, 2, 3, 4]

#code you solution using .collect here

~~~solution

nums.collect do |num|
	num * num
end

~~~validation

assert_equal(response, [1, 4, 9, 16])

~~~

%%%

%%%

### Code Challenge III: Using `.select`

Below we have a variable, `odds_and_evens`, set equal to an array of numbers. Use the `.select` enumerator to iterate over the array and return any even numbers. This about how to check if a number is even. Maybe google "how to check if a number is even ruby" or something like that...

~~~ruby

odds_and_evens = [1, 3, 2, 18, 5, 10, 24]

#code your solution using .select here

~~~solution

odds_and_evens.select do |num|
	num.even?
end

~~~validation

assert_equal(response, [2, 18, 10, 24])

~~~

%%%

%%%

### Code Challenge IV: Using `.find`

Below we once again have a variable, `odds_and_evens`, set equal to an array of numbers. This time, use the `.find` method to iterate over the array and return only the *first* array element that is *odd*.

~~~ruby

odds_and_evens = [1, 3, 2, 18, 5, 10, 24]

#code your solution using .find here

~~~solution

odds_and_evens.find do |num|
	num.odd?
end

~~~validation

assert_equal(response, 1)

~~~

%%%

%%%

### Code Challenge V: Using `delete_if`

Below we have a variable, `cats_and_dogs`, set equal to an array of strings that are either cats or dogs. We all know that cats and dogs don't get along. Iterate over the array and delete from it any items that are dogs.

~~~ruby

cats_and_dogs = ["cat", "cat", "dog", "cat", "dog", "dog"]

#code your solution using .delete_if

~~~solution

cats_and_dogs.delete_if do |pet|
	pet == "dog"
end

~~~validation

assert_match(response, ["cat", "cat", "cat"])

~~~

%%%

%%%

### Code Challenge VI: Using `include?`

Below we have a variable, `famous_cats`, set equal to an array of famous cats. Use the `.include?` method to check and see if the array includes the string "Maru".

~~~ruby

famous_cats = ["Maru", "Lil Bub", "Grumpy Cat"]

#code your solution using .indlude? here

~~~solution

famous_cats.include?("Maru")

~~~validation

assert_true(response)

~~~

%%%

%%%

### Code Challenge VII: Using `any?`

Below we have a variable, `quiet_and_loud`, that is set equal to an array of strings. Use the `.any?` method to iteratore over the array to determine if any of the words contained there are loud, or upcased.

~~~ruby

quiet_and_loud = ["hi", "HI", "shhh", "WHAT?!"]

#code your solution using .any? here

~~~solution

quiet_and_loud.any? do |word|
	word == word.upcase
end

~~~validation

assert_equal(response, true)

~~~

%%%


<a href='https://learn.co/lessons/enumerator-coding-challenge-new-repl-syntax' data-visibility='hidden'>View this lesson on Learn.co</a>
