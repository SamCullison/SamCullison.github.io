---
title: "Pattern Detector Program"
excerpt: "Python Program which generates subsequent numbers in a pattenr"
header:
  teaser: 
   
---

# Origin of the Pattern Project

I started working on this project at the end of my sophomore Spring Semester. I believed I could make a Python file which could extend an input list of numbers by 5 based on a pattern it "detected". I quickly realized that this was not possible for any list of numbers. Even if it were, it would not be accurate for every person using the program. This led to me changing my idea for the code, and instead creating a program which can generate the proceding 5 numbers of an established "head pattern". By "head pattern" I mean any pattern that you can create and elongate in your head as there are no rules for generating numbers based on trigonomic functions, logarithmic or exponential in this program. The only other rule is that the pattern must be present at least twice in the input. If this requirement is not fulfilled then the program will not have enough information to be accurate.

# Example Runs

What follows is an example run in which the constant addition, constant multiplication, iterative multiplication, iterative addition, and complex were tested.
The constant addition and multiplication are straightforwawrd. The iterative patterns are simply patterns such as +2, +3, -4 or *3, *2. Now the complex is where the program gets interesting, because it is able to continue a sequence with a pattern such as +2*3/2 and *(-5)-3. AN explanation for the functions that do this will follow below. 


<img src="/assets/img/Python Examples.png" alt="Example Patterns" style="width:900px;"/>
