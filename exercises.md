## Ruby Exercises

Put your solutions in a file called `ruby_methods.rb`. To run, type `ruby ruby_methods.rb` in the command line.

Exhausted your resources (google, classmates, etc) and still super stuck on a problem? Check out the [solutions](solutions.rb).

### Looping

Use a loop to do  the following:

1.) Write a method called `p_times` that takes a `statement` and a `num` puts the `statement` some `num` of times to the console.

2.) Write a method called `letter_count` to count letter occurence in a string, returned as a `Hash`.

3.) Write a method called `mock_me` that `gets` some input from the terminal and puts it until the users type `quit` or `q` in the terminal. (Be sure to remove trailing `\n`.)

4.) Write a method called `print_contacts` that takes a `hash` of `name` and `phone-number` key-value pairs and `puts` the `name` and `phone-number` for each contact.

5.) Write a method called `get_contact` that

  * takes a `contacts` hash,
  * prints the contacts,
  * prompts the terminal for a **new** `name` and a `phone` number,
  * and then adds the `name` and `phone` as a key value pair respectively if `name` is not already a contact, or
  * changes the phone number associated with `name` if the name is already a contact.
  * The `get_contact` method should `return` the `contacts` hash.
  
 *Hint:* No loop required for this one.

6.) Write a method called `get_contacts` that 

  * takes a `contacts` hash
  * keeps prompting the user to ask if they'd like to add a contact
  * lets them add a contact (as in the last exercise) if they say `y` or `Y`, then prompts them again
  * exits the program if they say `n` or `N`


### List exercises

#### Using `Enumerable#inject`

Sometimes you want to turn an array  into  one cumulative value.  In Ruby, the iterator method that does this is called `inject` or `reduce` (Ruby has two names for this same function).  In JavaScript, it's [`reduce`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce). You might also see it called `fold`.


[Docs for Enumerable#inject](http://ruby-doc.org/core-2.2.0/Enumerable.html#method-i-inject)  


Write a method for each exercise below that uses `Enumerable#inject`:

1.) Write a method called `get_sum` to find the `sum` of the values in an array.

2.) Write a method called `get_max` to find the `max` of the values in an array.

3.) Write a method called `get_min` to find the `min` of the values in an array.

4.) Write a method called `reverse_str` to reverse a string.

**Challenge**: *write a method called `partial_sums` that `push`es the partial sum of an array to a new list*

```
partial_sums([])
#=> [0]
partial_sums([5])
#=> [0, 5]
partial_sums([5,6,7])
#=> [0, 5, 11, 18]
```

#### Using `Array#map`
[Docs for Array#map] (http://ruby-doc.org/core-2.2.0/Array.html#method-i-map)

Write a method for each exercise below that uses `Array#map`:

1.)  Write a method called `multiply_by` that takes a number and returns an array of numbers multiplied by that number.

2.)  Write a method called `reverse_each` that takes an array of words and returns an array of reversed words.

3.)  Write method called `get_responses` that takes an array of questions (strings) and returns an array of responses input from the console for each question. (Hint: you will need to use `gets.chomp` and `puts` )

### Method Exercises

1.) Write a method to compute the `factorial` of a number.

2.) Write a method to check if a number is a palindrome.

3.) Write a method to `reverse` a word.
