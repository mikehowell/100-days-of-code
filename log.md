# 100 Days Of Code - Log

### Day 0: April 30, 2018

**Today's Progress**: Created code and unit tests to reverse an array without using another array.

**Thoughts**: This was way harder than I expected.  I'm not happy with the naming but I created a separate class with a method to do the reversing of the string input.  I expect that there is a better way to acheive this too by calling the [Linq reverse method](https://msdn.microsoft.com/en-us/library/bb358497(v=vs.110).aspx) but I'm not sure how to acheive this.  I also created a unit test and want to create unit tests for 100 days of code.

**Link to work**: [Day 0](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day0).

### Day 1: May 1, 2018 ###

**Today's Progress**: Created code and unit tests to produce a sample output based on two integers as input.

**Thoughts**: This was a little easier after day 0 but I ended up creating the repo with a different tree structure.  I'm not clear why.  I need to refactor this.  I also added a unit test which fails, again it's unclear why, as both the result from the method call and the execpted result appear to be the same visually in debug mode i.e. both a generic List<int> with the same number if items and each item has the same value.  Perhaps there is another way to compare generic lists.
  
**Link to work:** [Day 1](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day1/Day1).
  
**UPDATE: Day 1:** Unit tests now passing.  Collections should be compared in unit tests using CollectionsAssert.AreEqual as per this Stack Overflow [article](https://stackoverflow.com/questions/11055632/how-to-compare-lists-in-unit-testing).

### Day 2: May 2, 2018 ###

**Today's Progress**: Created code and unit tests to return Maximum and Minimum Temperatures from an array of floats.

**Thoughts**: This challenge was easier that the previous days and in the class I included two public properties.

**Link to work**: [Day 2](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day2/MinMaxTemperature).

### Day 3: May 3, 2018 ###

**Today's Progress**: Created code and unit tests to return a sorted list of integers from a list of 3 integers.

**Thoughts**: I feel I cheated a little on this one by using the sort method on a list in the System.Collections.Generic.
It was still difficult trying to do it in a class.  
I wouldn't mind trying to implement an actual sorting algorithm in a class rather than using the sort method.

**Link to work**: [Day 3](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day3).

### Day 4: May 4, 2018 ###

**Today's Progress**: Created code and unit tests to return an integer in an Indian Rupee Format.

**Thoughts**: Today felt easier.  However, the class is simply a method that converts the int to a string and then returns an appropriate formatted string from substrings of the string.

**Link to work**: [Day 4](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day4).

### Day 5: May 5, 2018 ###

**Today's Progress**: Created code and unit tests to return prime factors for a number.

**Thoughts**: I needed to Google prime factorization and found some interesting worked examples on [StackOverflow](https://stackoverflow.com/questions/5872962/prime-factors-in-c-sharp) which formed the basis for completing this exercise.

**Link to work**: [Day 5](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day5).

### Day 5.1: May 5, 2018 ###

**Today's Progress**: Created code and unit tests to remove a character from a string.

**Thoughts**: I decided to do another challenge today.  This one seemed harder that it should have been.  There doesn't appear to be built in .Net method to do this.  I used two Lists, one to contain the string and the other to take the characters that didn't need removing.  Finally I iterated over this List to "convert" it to a string.  There's bound to be a much earier way to do this.

**Link to work**: [Day 5.1](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day5.1).

### Day 6: May 6, 2018 ###

**Today's Progress**: Created code and unit tests to test validity of 10 digit ISBN number.

**Thoughts**: This was fun challenge and a good candidate for extension to test validity of 13 digit ISBN numbers too.  I also used a try catch block and added basic exception handling for a case when a string that is not 10 characters long is entered.  I had a problem trying to get the unit test for this to work.  After adding the [ExpectedException(typeof(Exception))] decorator to the test method, I also had to add a throw to the catch block to get the unit test to pass.
Useful links to articles on ISBN:
1. [Wikipedia](https://en.wikipedia.org/wiki/International_Standard_Book_Number)
2. [Instructables](http://www.instructables.com/id/How-to-verify-a-ISBN/)

**Link to work**: [Day 6](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day6).

### Day 6.1: May 6, 2018 ###

**Today's Progress**: Created code and unit tests to return the sum of all multiples of 3 and 5 less than 1000.

**Thoughts**: I had time to tackle another challenge so attempted this rather easy one.  The effort to write the unit test felt wasted.

**Link to work**: [Day 6.1](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day6.1).

### Day 7: May 7, 2018 ###

**Today's Progress**: Created code and unit tests to test if a number is a Strong Number, which is one where the factorial of the individual digits adds up to the number itself.  For example, 145 = 1! + 4! + 5! = 1 + 24 + 120.

**Thoughts**: I'm not sure that I implemented the class for this one in a good way but I had fun.  I used private fields, a constructor with a parameter, a number of private methods and a public method to return true or false depending on whether the number is strong or not.  I also set up some private fields ahead of the TestMethods in UnitTests, feeing up the UnitTests to instatiate an instance of the StrongNumber class and then make an Assertion based on the call to the method, IsStrongNumber.

**Link to work**: [Day 7](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day7).

### Day 8: May 8, 2018 ###

**Today's Progress**: Created code and unit tests to sum all the positive integers in an array.

**Thoughts**:  I still struggle naming things but at least the code seems to flow a little easier.

**Link to work**: [Day 8](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day8).

### Day 9: May 9, 2018 ###

**Today's Progress**: Created code and unit tests to check a leap year.

**Thoughts**: I picked an easy challenge today as I spent a lot of time waiting for Visual Studio to update before I could progress.  I managed to create the code to fulfill the challenge without cheating but resoted to multiple nested ifs which is probably frowned upon by more experienced developers and to be honest, looks ugly.  I did find a nice way to acheive the same result in an if else block from [StackOverflow](https://stackoverflow.com/questions/725098/leap-year-calculation).  Which I included in my method but commented out.

**Link to work**: [Day 9](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day9).

### Day 10: May 10, 2018 ###

**Today's Progress**: Created code and unit tests to return remainder when dividing by 13.

**Thoughts**: The maths of this was a little complex to get to grips with at first.  I also cheated a little on the unit tests in that I created two assertions in one test and populated them with values on the fly, rather than setting variables with these values and then using the variables in the assert, which I think looks better and is generally more readable.

**Link to work**: [Day 10](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day10).

### Day 11: May 11, 2018 ###

**Today's Progress**: Created code and unit tests to test validity of an IPV4 address.

**Thoughts**: I worked through this challenge without any Googling, using only the examples for guidance.  I used the examples to validate the results via the unit tests but perhaps I could have written the unit tests first!

**Link to work**: [Day 11](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day11).

### Day 12: May 12, 2018 ###

**Today's Progress**: Created code and unit tests to convert hyphen or underscore delimited words into camel casing.

**Thoughts**: This was a nice easy challenge for a Saturday.  I'm still sure that there could be better ways to acheive this.

**Link to work**: [Day 12](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day12).

### Day 12.1: May 12, 2018 ###

**Today's Progress**: Created code and unit tests to return the sum of all even numbers in a Fibonacci Sequence up to four million.

**Thoughts**: This was way harder than it looked at first sight but doing research lead me to explore using a Linq (Lambda) expression and the _yield_ key word which I'm still not sure about.

**Link to work**: [Day 12.1](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day12.1).

### Day 13: May 13, 2018 ###

**Today's Progress**: Create code and unit tests to return the smalled and largest possible sums from an array of numbers.

**Thoughts**: This challenge was fun.  I extended it to allow the input of as many numbers as the user wants by using the param key word on the contructor method.  Oddly, without including a parameterless contructor, instantiating the class without any inputs didn't cause the compiler to complain.  I'm not sure why!

**Link to work**: [Day 13](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day13).

### Day 14: May 14, 2018 ###

**Today's Progress**:  This was extremely challenging and not finished!

**Thoughts**: This challenge should have been completed two days ago but a migraine put an end to the work.  Last I went to wattch Deadpool 2 - definitely worth missing an eveing coding for.  I'll try and add another challenge tonight (17 May).

**Link to work**: [Day 14](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day14).

### Day 15: May 17, 2018 ###

**Today's Progress**:  Created code with exception handling and unit test to turn seconds into HH:MM:SS format.  This was fun and easy.

**Thoughts**:  I felt the need to an easier challenge to help boost me after day 14's failed attempt.  This one fitted nicely!  I added exception handling and a unti test that tests for the exception.

**Link to work**: [Day 15](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day15).

### Day 16: May 18, 2018 ###

**Today's Progress**:  I created this challenge myself as a way to generate random Lotto numbers.  

**Thoughts**:  I felt this would be an easy challenge but I had fun with it and was able explore using properties with private setters, a constructor to set the property values only if they were valid, otherwise throw an exception.  The unit tests were challenging but I tested exceptions for each input parameter, that the count of random numbers returned was correct and that they are all different.

**Link to work**: [Day 16](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day16).

### Day 17: May 19, 2018 ###

**Today's Progress**:  Created a grade rounding system.

**Thoughts**:  This challenge was relatively straight forward. However, the class feels a little bloated and has a number of private methods and a private property.  There might be a better way to split this out into a number of sub classes, which could be a valuable exercise.  There is also quite a bit of error handling around the inputs and unit tests to test both valid rounding and that each exception is correctly thrown.

**Link to work**: [Day 17](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day17).

### Day 18: May 20, 2018 ###

**Today's Progress**:  Created a phone number validator using a regular expression.

**Thoughts**: This was a simple challenge but took a while to figure out the regular expression.

**Link to work**: [Day 18](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day18).

### Day 19: May 21, 2018 ###

**Today's Progress**: Tested whether a number is Disarium or not.

**Thoughts**: This challenge looked harder than it was and in the end, I create a class with a single method and nothing else to solve the challenge.  I found an interesting way to split a number into and array of it's digits.  I suspect this could be condensed into iterating over the stack and working out the sum of the digits to their respective powers rather than introducing an array.  Perhaps that's part of a refactoring challenge.

**Link to work**: [Day 19](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day19).

### Day 20: May 22, 2018 ###

**Today's Progress**: Created a Stopwatch class with proper encapsulation and error handling.

**Thoughts**: This was a good challenge and more of what I feel I need to do to practice for the MS exam.

**Link to work**: [Day 20](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day20).

### Day 21: May 23, 2018 ###

**Today's Progress**: Created an abstract DbConnection class and two classes that inherited from this abstract class.

**Thoughts**: I had the chance to practise setting different access modifiers but was not able to fiugre out how to implement unit tests for methods that don't have any implementation but just write out to the console (as pseudo implementation).  There is opportunity here to enhance this implementation by implementing a timer and if this exceeds the timeout for establishing a db connection, throw and exception.

**Link to work**: [Day 21](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day21).

### Day 22: May 24, 2018 ###

**Today's Progress**: Followed on from yesterday by creating a DbCommand class that takes a DbConnection and command to be exectuted against the database.

**Thoughts**: This was interesting to be able to pass an object (DbConnection) as a parameter of the DbCommand contructor method.  My mindset so far has been that parameters to methods are value types rather than reference types.  I need to get my head around this idea and embrace it to progress my coding skills.

**Link to work**: [Day 22](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day22).

### Day 23: May 25, 2018 ###

**Today's Progress**: Created a class to count the number of times a digit can be found in the squares of a range of numbers.

**Thoughts**: This is another example of where I've needed to split a digit into an array of it's individual numbers.  There must be an easier way to achieve this.

**Link to work**: [Day 23](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day23).

### Day 24: May 26, 2018 ###

**Today's Progress**: Created a guessing game app.

**Thoughts**: I played around with separate classes, where one generates a random number in the constructor and the game class takes the random number class as input.  This may not have been the best approach but still a useful exercise.  I had problems creating unit tests for these classes.

**Link to work**: [Day 24](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day24).


### Day 25: May 27, 2018 ###

**Today's Progress**: Created string pattern based on integer input.

**Thoughts**: This was very easy but I had a chance to play around with string builder.  String builder is very powerful.

**Link to work**: [Day 25](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day25).

### Day 26: May 28, 2018 ###

**Today's Progress**: Added methods to C# class to return correct change based on amount paid and cost.

**Thoughts**: This was very hard and took three days of gnawing at it to get something that works, in that it returns the right change but the unit tests for some reason don't pass, except the one that returns and empty list of change where not change is expected and I'm not sure why.  This is a problem for another time.  Additionally, the way I calculated the change is very long winded.  I know there are better ways, I've seen them on the internet, I just don't understand them enough to implement my own.  This problem is very close to what I'd expect in the real world i.e. high, can you finish off this code for project X as developer Y is part way through but on sick leave today.......

**Link to work**: [Day 26](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day26).

### Day 27: May 31, 2018 ###

**Today's Progress**: Added code to method to correctly return Roman Numeral for integers between 1 and 4999.

**Thoughts**:  This was relatively straight forward and a nice use for recursion.  It's provided an idea on how to refactor the previous challenge.

**Link to work**: [Day 27](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day27).

### Day 28: June 1, 2018 ###

**Today's Progress**: Added code to method to correctly return integer from Roman Numeral string.

**Thoughts**:  This was a good challenge and a nice way to end the week.

**Link to work**: [Day 28](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day28).

### Day 29: June 2, 2018 ###

**Today's Progress**: Added code to method to translate English word into Pig Latin.

**Thoughts**: This was a good string manipulation exercise and initially I was iterating over arrays of characters but soon figured out that there are some useful string methods and can be used to easily solve the challeng like string.IndexOfAny(char[]).  I was not able to get the **extra credit** unit tests to pass as these input sentences with capitalization and commas and full stops that need to be accounted for.  I will extend this method to acheive this.

**Link to work**: [Day 29](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day29).

### Day 30: June 3, 2018 ###

**Today's Progress**: Updated code from yesterday to attempt to get addtional **extra credit** unit test to pass.

**Thoughts**: This is challenging.  I'm not able to get one unit test to pass the has the word quick in it.  The unit test expects that quick becomes ickquay i.e. the q and u travel as a unit but taking the code takes the index of the first vowel as the u and returns uickqay.  I'm guessing this is meant to be an exception rather than an error with the unit test.  I need to figure out how to code for this exception.  What if a word staring with qu doesn't contain any other vowels?  Do such English words exist.  Also, this exception needs to be catered for when I write the other method to translate back from Pig Latin to English!

**Link to work**: [Day 30](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day29).

### Day 31: June 4, 2018 ###

**Today's Progress**: Started updating method to convert Pig Latin to English.

**Thoughts**:  This is quite hard but I want to try solve the thing without Googling an answer.  It's easy enough to translate words ending in way that start with a vowel by dropping way with some exceptions like orldway which should translate to world.  Words ending in ay are more difficult.  How do you ascertain how many letters at the end need to be moved to the begining?

**Link to work**: [Day 31](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day30).

### Day 32: June 5, 2018 ###

**Today's Progress**: Updated method for converting Pig Latin to English.  The base unit tests now pass.

**Thoughts**: The method now returns some English words but not all.  I cannot get the **extra credit** unit tests to pass so some more work needs to be done to tackle this.

**Link to work**: [Day 32](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day30).

### Day 33: June 6, 2018 ###

**Today's Progress**: Updated encode and decode methods for Caesar Cipher.

**Thoughts**: This was way less challenging than the Pig Latin converter which is still not finished BTW!  I had extra time so did both the encode and decode methods in one sitting.

**Link to work**: [Day 33](https://github.com/mikehowell/100-days-of-code-the-challenges/blob/master/solutions/day31).

### Day 34: June 7th & 8th, 2018 ###

**Today's Progress**: Completed simple method to determine call duration based on variable cost per minute.

**Thoughts**: I started this yesterday (7th June) and although this was very simple, needed to finish off on the 8th as I needed time to prep for a C# presentation on interfaces for our lunchtime C# study group that happens each Friday.  It was good to have to create unit tests from scratch.  The test method naming needs work. 

**Link to work**: [Day34](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day32).

### Day 35: June 9th, 2018 ###

**Today's Progress**:  Completed another simple challenge to return Pling, Plang or Plong based on the factors of a number.

**Thoughts**:  Initially this looked daunting but on starting, I quickly realised this is very similar to the Fizz Buzz challenge.

**Link to work**: [Day 35](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day33).

### Day 36: June 10th, 2018 ###

**Today's Progress**:  Completed a encoding and decoding challenge for Rail Fence Cipher.  

**Thoughts**: This was tricky and more like the types of problems I need to continue to practice.  This was started yesterday, hence marked as day33.1.

**Link to work**: [Day 36](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day33.1).

### Day 36: June 10th, 2018 ###

**Today's Progress**:  The date isn't wrong for this one.... I completed a second easy challenge.  This was to return the longest work in a sentence.

**Thoughts**:  My initial take on this is that it was tricky, especially as the words need to exclude punctuation.  I tried a silly way initially to remove punctuaion before discovering that the char type has a static method IsPunctuation.  Using this, it's quite easy to remove any punctuation from a word by splitting it into it's characters and iterating over them.

**Link to work**: [Day 36](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day34).

### Day 37: June 11th, 2018 ###

**Today's Progress**: Created code to test if two "encrypted" strings are the same.

**Thoughts**: this was an interesting challenge in that it mixed dealing with strings and numbers to form an encrypted string, as always, there are probably shorter more succinct ways to acheive the same result but I'm happy with the outcome.  The code reads well and I've broken it up into a few methods that each do a separate task.

**Link to work**: [Day 37](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day35).

### Day 38: June 13th, 2018 ###

**Today's Progress**: Created code to reduce string as per challenge instructions.

**Thoughts**: I started this yesterday and struggled with it, in spite of it being relatively simple.  Arrays are tricky!

**Link to work**: [Day 38](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day36).

### Day 39: June 14th, 2018 ###

**Today's Progress**: Created code to determine if an addition equation is a Turing equation i.e. when revered, it is correct.

**Thoughts**: This one wasn't too difficult but I've had a bunch of ideas on how to solve this differently that I'd like to explore.

**Link to work**: [Day 39](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day37).

### Day 40: June 26th, 2018 ###

**Today's Progress**: Created code to calculate values for uniform strings.

**Thoughs**:  I spent a few hours each night of the last few days trying to figure this one out.  The tricky part is working out how to return the uniform strings from a string of lower case letters i.e. for string "aabccdccc", the uniform contiguous substrings are a, b, c, d, aa, cc, ccc.  I finally solved this using a stack to track the contiguous substrings but as always, I'm sure there are better ways to do this.

**Link to work**: [Day 39](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day38).

**NOTE**: It's been over a week since I submitted anything to GitHub as part of the 100 days of code challenge.  I've been coding during this time on a corporate challenge which I've not been able to share here.  I was only able to complete half of the corporate challenges in the week but won the competition (more by default than by skill as I was the only one to submit the work I did but the past 38 days of coding certainly helped).

