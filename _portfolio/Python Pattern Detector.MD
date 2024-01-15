---
title: "Pattern Detector Program"
excerpt: "Python Program which generates subsequent numbers in a pattenr"
header:
  teaser: /assets/img/Example_Patterns.jpg
   
---

# Origin of the Pattern Project

I started working on this project at the end of my sophomore Spring Semester. I believed I could make a Python file which could extend an input list of numbers by 5 based on a pattern it "detected". I quickly realized that this was not possible for any list of numbers. Even if it were, it would not be accurate for every person using the program. This led to me changing my idea for the code, and instead creating a program which can generate the proceding 5 numbers of an established "head pattern". By "head pattern" I mean any pattern that you can create and elongate in your head as there are no rules for generating numbers based on trigonomic functions, logarithmic or exponential in this program. The only other rule is that the pattern must be present at least twice in the input. If this requirement is not fulfilled then the program will not have enough information to be accurate.

# Example Runs

What follows is an example run in which the constant addition, constant multiplication, iterative multiplication, iterative addition, and complex were tested.
The constant addition and multiplication are straightforwawrd. The iterative patterns are simply patterns such as +2, +3, -4 or *3, *2. Now the complex is where the program gets interesting, because it is able to continue a sequence with a pattern such as +2*3/2 and *(-5)-3. An explanation for the functions that do this will follow below. 


<img src="/assets/img/Python Examples.png" alt="Example Patterns" style="width:900px;"/>

# The Complex Iterative Pattern

Creating the constant, iterative and even complex functions was straightforward. However, combining the key attributes from each of these into the complex iterative function was difficult. Instead of a simple complex pattern such as *2+1, now the program was dealing with *2+1, *-3+7, -10. I defined this example as a 3 "step" pattern because it has 3 alternating rules, but the function was made to handle any number of steps in the given pattern. For example a run with a pattern of *2+1,-10,*3,-2, follows. 
Given Input: 12, 25, 15, 45, 43, 87, 77, 231, 229, 459, 449, 898

<img src="/assets/img/Complex Pattern Ex.png" alt="ex complex pattern" style="width:500px;"/>

# How the Complex Pattern Works

Defining the function to extend a complex pattern suprised me. Before testing the sequences I believed that the function would have to iterate through different variations of pattern differences and pattern multiples (using the list_difference() and list_multiplier() functions). I quickly learned that this was not the case, and that the function only had to use one difference of the original data, followed by a multiplier of this new list. Using these two lists and the original data proved to be enough. With these lists the program is able to use the mult to extend the lin, and then use the extended lin to generate the next number in the original sequence. The iterative part of the complex function needed much more work (the original list had to be broken down further before using the difference and multiplier functions), but the process was the same.

# Future Work

Although the program works as I envisioned there are a couple details/functionalities I would like to add..
* First, the complex iterative capability requires 2x the pattern length to work properly. For example, a two step pattern (such as x2,-2) requires 4 input numbers. For a two step pattern this is not a big deal, but in the future I would like to change the program so that it requires the minimum amount of input. This is possible, and I know how to do it, it will just take changing the core code of the complex pattern
* Second, I want this program to extend any pattern. Now there are good ways and bad ways to do this, but the complex pattern could augmented to perform this task with very minor changes. All it would take is assuming that the pattern is only what has been presented, nothing more and nothing less. For example is you wanted a pattern of *3,-2,+1 then all you would have to input is 1, 3, 1,2.
* Finally, obviously the user can make simple addition and multiplication errors when putting their head pattern into the computer. In the future I would like to make the program capable of adjusting to slight deviations from a prescibed pattern, and thus carrying on as normal. Adding this will be the most difficult capability but I believe it will make the program much more useful.

# The Program Itself 
The Pattern Detector program was made in Pycharm and a pdf of the code is available below.

<a href="username.github.io/Synthetic Biology Final Report.pdf" target="_blank">PDF.</a>

