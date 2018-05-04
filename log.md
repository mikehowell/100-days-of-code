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

**Today's Progress**: Create code and unit tests to return prime factors for a number.

**Thoughts**: I needed to Google prime factorization and found some interesting worked examples on [StackOverflow](https://stackoverflow.com/questions/5872962/prime-factors-in-c-sharp) which formed the basis for completing this exercise.

**Link to work**: [Day 5](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day5).
