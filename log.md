# 100 Days Of Code - Log

### Day 0: April 30, 2018

**Today's Progress**: Created code and unit tests to reverse an array without using another array.

**Thoughts:** This was way harder than I expected.  I'm not happy with the naming but I created a separate class with a method to do the reversing of the string input.  I expect that there is a better way to acheive this too by calling the [Linq reverse method](https://msdn.microsoft.com/en-us/library/bb358497(v=vs.110).aspx) but I'm not sure how to acheive this.  I also created a unit test and want to create unit tests for 100 days of code.

**Link to work:** [Day 0](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day0)

### Day 1: May 1, 2018 ###

**Today's Progress**: Created code and unit tests to produce a sample output based on two integers as input.

**Thoughts:** This was a little easier after day 0 but I ended up creating the repo with a different tree structure.  I'm not clear why.  I need to refactor this.  I also added a unit test which fails, again it's unclear why, as both the result from the method call and the execpted result appear to be the same visually in debug mode i.e. both a generic List<int> with the same number if items and each item has the same value.  Perhaps there is another way to compare generic lists.
  
  **Link to work:** [Day 1](https://github.com/mikehowell/100-days-of-code-the-challenges/tree/master/solutions/day1/Day1)
  
  **UPDATE: Day 1:** Unit tests now passing.  Collections should be compared in unit tests using CollectionsAssert.AreEqual as per this Stack Overflow [article](https://stackoverflow.com/questions/11055632/how-to-compare-lists-in-unit-testing).
