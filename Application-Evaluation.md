# Application Evaluation 
#### Evaluating the Code Structure and Characteristics of an Application Implementing Programming Paradigms.
## Contents
[I. Contents](#contents)   
[II. Introduction](#introduction)   
[III. Code](#code)   
[IV. Paradigms](#paradigms)   
[V. Code Structure and Characteristics](#code-structure-and-characteristics)   
[VI. Evaluation](#evaluation)   
[VII. Conclusion](#conclusion)   
[VIII. References/Bibliography](#references)   

## Introduction

### Code 
The following is the code that will be evaluated in this report:
 
## Paradigms
As covered in a previous report, the three different paradigms have different approaches to the programming of an application. The different approaches that each paradigm has are the following:

The Object-Orientated Programming (OOP) approach handles problems by using objects. These objects include attributes and different behaviours, which can interact with one another by calling methods onto other objects. The process generally consists of a class being defined that acts a template, which is then filled with attributes and methods and used in the program. 

The Event-Driven Programming (EDP) approach handles problems by using events. The process involves having an event, an object to act on the event, and an event handler/listener which will be triggered when the event occurs. Event functions usually work by having an event listener, which is activated by the event, which will then call the specific function linked to the event. 

The Procedural Paradigm has an approach which is much more linear than OOP or EDP, it does not react to events and does not have templates for different instances of the same code. However, it is still possible to have the same functionality as the other paradigms, just in a much more complex and long-winded approach.

## Code Structure and Characteristics
The program is sectioned into different parts, the different functions that are used for the game are near the top, while the variables that the game uses are all defined near the bottom. The game has a main function called ‘GameLoop’ this makes use of the other functions in order to refresh the game canvas to update what is happening in the game on screen.

The program relies on events, which are part of the event-driven paradigm. The main event is the ‘mousemove’ event that takes place on the game window which acts as the event handler (window.addEventListener ("mousemove", MousePos)), using the ‘MousePos’ function to store the location of the mouse within the game window. The mouse location on the game window is a vital part of the game, which affects all other functions.

For the other parts of the code, a more object-orientated approach is taken. While the actual code is not written as it normally would be in object-orientated programs, the concepts and approach are similar. For example, the player and enemy are defined by what would be considered ‘attributes’ (context.fillStyle, context.fillRect). However, instead of having a class such as ‘player()’ they are defined as variables at the end of the code, with all the other variables. 

## Evaluation
The code in this program is functional and works as intended. However, the approach to the coding could be improved by taking a different approach. The code was written using mostly EDP, with aspects of OOP. This could have been done by using EDP and actual aspects of OOP. In the code, objects, classes and methods are not really utilised as they could have been. For example, instead of setting all the variables at the bottom of the code, the player and the enemy could have been two different objects using the same class, as they are the same entity but with different attributes. This would simplify the code, as well as help organise it better.

A completely different approach could have been taken to create the program altogether, instead of using OOP and EDP together, a single paradigm could be used, or even a different paradigm such as the Procedural Paradigm. This would result in a completely different code, but with the same outcome. This may or may not result in a more efficient implementation of the program.

## Conclusion
To conclude, it can be seen that EDP and aspects of OOP paradigms are used in this program to meet the requirements of the client. While the application works as intended, the usage of paradigms in the program could be improved or revised. Taking a different approach to program, could lead to a more efficient development process, while still leading to the same outcome. 

## References
Traceball program. Available at:  https://github.com/Fabijuss/trace-ball/blob/master/source/index.html
Paradigm report. Available at: https://github.com/Fabijuss/Programming/blob/master/Paradigms.md




