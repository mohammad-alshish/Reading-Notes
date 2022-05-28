## Read: Class01

For our first class I resocres that we meant to Skim and summraize are the following:
1. [Pain and Suffering](https://codefellows.github.io/code-401-python-guide/curriculum/class-01/notes/pain_suffering)
2. [Begineners Guide For BigO](https://rob-bell.net/2009/06/a-beginners-guide-to-big-o-notation/)
3. [Names and Values in Python](https://www.youtube.com/watch?v=_AEJHKGk9ns)
4. [Awsome Python Enviroment](https://www.youtube.com/watch?v=_AEJHKGk9ns)
5. [Phyton Moduke Of The Week](https://pymotw.com/3/index.html)


## My Summary

***After going through the resources above we can summriaze them like this***

### **What is Big O Notation, and why does it matter ?**

“Big O notation is used in Computer Science to describe the performance or complexity of an algorithm. Big O specifically describes the worst-case scenario, and can be used to describe the execution time required or the space used (e.g. in memory or on disk) by an algorithm.
and for these how love math we can say is a mathematical notation that describes the limiting behavior of a function when the argument tends towards a particular value or infinity. It is a member of a family of notations invented by Paul Bachmann, Edmund Landau, and others, collectively called Bachmann–Landau notation or asymptotic notation.”

### **Formal Definition of Big O notation (Best Example For Big O)**
Once upon a time there was an Indian king who wanted to reward a wise man for his excellence. The wise man asked for nothing but some wheat that would fill up a chess board.

But here were his rules: in the first tile he wants 1 grain of wheat, then 2 on the second tile, then 4 on the next one…each tile on the chess board needed to be filled by double the amount of grains as the previous one. The naïve king agreed without hesitation, thinking it would be a trivial demand to fulfill, until he actually went on and tried it…So how many grains of wheat does the king owe the wise man? We know that a chess board has 8 squares by 8 squares, which totals 64 tiles, so the final tile should have 2⁶⁴ grains of wheat. If you do a calculation online, you will end up getting 1.8446744*10¹⁹, that is about 18 followed by 18 zeroes. Assuming that each grain of wheat weights 0.01 grams, that gives us 184,467,440,737 tons of wheat. And 184 billion tons is quite a lot, isn’t it?

The numbers grow quite fast later for exponential growth don’t they? The same logic goes for computer algorithms. If the required efforts to accomplish a task grow exponentially with respect to the input size, it can end up becoming enormously large.

Now the square of 64 is 4096. If you add that number to 2⁶⁴, it will be lost outside the significant digits. This is why, when we look at the growth rate, we only care about the dominant terms. And since we want to analyze the growth with respect to the input size, the coefficients which only multiply the number rather than growing with the input size do not contain useful information.

### **Big O notation some examples**

1. O(1) describes an algorithm that will always execute in the same time (or space) regardless of the size of the input data set.

2. O(N) describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set

3. O(N²) represents an algorithm whose performance is directly proportional to the square of the size of the input data set. This is common with algorithms that involve nested iterations over the data set. Deeper nested iterations will result in O(N³), O(N⁴) etc. 4.O(2^N) denotes an algorithm whose growth doubles with each addition to the input data set. The growth curve of an O(2^N) function is exponential — starting off very shallow.

### **Logarithms** 
Logarithms or log: A mathematical concept/expression that’s used a lot in Computer Science and it’s the inverse (flip) of exponentials, and they’re used to answer the question: How many times must one “base” number be multiplied by itself to get some other particular number or (what power you have to raise to, to get another number) or we can also define it as The power (or exponent) to which one base number must be raised (multiplied by itself) to produce another number.

Example: How many times must a base of 20 be multiplied by itself to get 8,000? The answer is 3 (8000 = 20 × 20 × 20). So the logarithm base 20 of 8,000 is 3. It’s represented using a subscript (small number) to the lower right of the base number. So the statement would be log20(8,000) = 3.

log20(400) is like asking “How many 20s do we multiply to get 400? which is 2(20 * 20). So log20(400) = 2

### **How Python Dealing with the Variables and values**

So the idea here is to understand the how PYTHON deals with the variables and how  we can use this in the best way possible to make  the codes we write more effective and easier for debugging. Now lets build some ground here :
1. Variable names may contain letters, digits (0-9) or the underscore character _.
2. Variable names must begin with a letter from A-Z or the underscore _ character. Either lowercase or uppercase letters are acceptable.
3. Variable names may not be a reserved word in Python.
4. Many names can refer to one value
5. Names are assigned independently

So You need to understand the flow that the names you choose will go throygh while writing the code,So I strongly recommend  to Use this site [pythontutor](https://pythontutor.com/)

Write few codes and see with your own eyes what happens for the names and the values.


## **Things I want to know more about**

### 1. I want to know more about Big O cases.
### 2. I want to know how coding smimlir for math concepts that I have.