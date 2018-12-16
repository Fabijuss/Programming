# Implementation of an Algorithm
#### Examining the Implementation of an Algorithm and Evaluating the Relationship Between the Written Algorithm and the Code Variant.
## Contents
[I. Contents](#contents)   
[II. Introduction](#introduction)   
[III. Algorithm](#algorithm)   
[IV. Final Code](#final-code)   
[V. Implementation and Relationship](#implementation-and-relationship)   
[VI. Conclusion](#conclusion)   
[VII. References/Bibliography](#references)   

## Introduction
This short report will cover the implementation and the relationship between the written algorithm and the code variant. The algorithm and the written code will be compared to see how the code has been implemented, and the relationship between the two will be evaluated.
 
## Algorithm

![High or low flowchart](https://i.imgur.com/b6kF6yM.png)

The above image is of the flowchart algorithm used for the Higher or Lower program. 

## Final Code

![Final Code](https://i.imgur.com/MczB4Jk.png)
 
The above image is of the final code used in the program.

## Implementation and Relationship
For this project, the code was implemented as closely to the flowchart as possible. This was done in order to follow the plan laid out for the project, so that all of the user requirements are met. 

The code has a number of different sections, which were planned in the flowchart. The first section was the generation of random numbers, one for both the player and the computer. This was carried out using C++, which created a random generated seed using time as the method of randomisation. However, the method used to do this would differ in most programming languages and the approach to creating randomly generated numbers can differ in a number of ways.

The next section involved creating a loop which would only accept certain inputs from the user. The flowchart portrays this as a simple loop, which takes an input, checks if it’s valid and either asks for another input or continues based on the input. The code implements this is as a ‘do while’ loop, this could be carried out in a number of different methods, using different loops. This would also vary depending on the programming language used.

The third part of the algorithm was the win/loss condition check. This was carried out by comparing the two randomly generated values, along with the guess of the player. This resulted in a number of conditions that must be checked in order to confirm that the player has won/lost/tied. The code checks both win conditions in one line, the same being with the loss conditions. This could have been carried out in a number of different methods, such as using multiple if statements for each condition or in the form of a while loop which checks the conditions. This logic would be similar in most programming languages, the only thing that may differ is the order of the code or operators used.

The final part of the algorithm required the application to restart. This was carried out by using a while loop in the code which started the main code algorithm again, or did nothing – which would stop the code. This could have been carried out in a few different ways, such as using functions for the restart section and the main code. This may also differ in different programming languages, as doing ‘nothing’ could lead to the application hanging or resulting in an error. Instead, the application could do a system exit to end. 

While most of the code is accurate to the flowchart, one area was overlooked during the creation of the flowchart. This is the section which displays the actual numbers which were generated. This was done by displaying the value of the numbers after showing the results of the game. Which would work the same in most programming languages.

## Conclusion
To conclude, the flowchart algorithm was followed closely during the creation of the final code. The interpretation of the algorithm into the actual code may vary in a number of different sections of code, such as the logic and the methods used to carry out some functions, i.e. number generation. The code would also differ if it were implemented in a different language, as some of the logic used may not be compatible with other languages. However, the overall algorithm could be implemented in a number of different languages if it were adapted to suit them.

## References
Higher or Lower program. Available at: https://github.com/Fabijuss/High-Low



