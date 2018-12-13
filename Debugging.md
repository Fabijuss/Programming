# Debugging
#### Outlining the Debugging Process and Debugging Facilities in an IDE.
## Contents
[I. Contents](#contents)   
[II. Introduction](#introduction)   
[III. Debugging](#debugging)   
&nbsp;&nbsp;[III.1 What is debugging?](#what-is-debugging)   
&nbsp;&nbsp;[III.2 Debugging process](#debugging-process)   
&nbsp;&nbsp;&nbsp;&nbsp;[III.2.1 Identifying a bug](#identifying-a-bug)   
&nbsp;&nbsp;&nbsp;&nbsp;[III.2.2 Classifying a bug](#classifying-a-bug)   
&nbsp;&nbsp;&nbsp;&nbsp;[III.2.3 Understanding a bug](#understanding-a-bug)   
&nbsp;&nbsp;&nbsp;&nbsp;[III.2.4 Repairing a bug](#repairing-a-bug)   
[IV. Debugging Facitilies](#debugging-facilities)   
&nbsp;&nbsp;[IV.1 Breakpoints](#breakpoints)   
&nbsp;&nbsp;[IV.2 Output Console](#output-console)   
&nbsp;&nbsp;[IV.3 Diagnostics](#diagnostics)   
&nbsp;&nbsp;[IV.4 Variable changing](#variable-changing)   
&nbsp;&nbsp;[IV.5 Call stack viewing](#call-stack-viewing)   
[V. Building a Robust Application](#building-a-robust-application)   
[VI. Conclusion](#conclusion)   
[VII. References/Bibliography](#references)   

## Introduction
This short-form report will cover the process of debugging an application, and the debugging facilities available in Integrated Development Environments. Debugging will be defined and the process of debugging will be explored in this report.

The debugging facilities found in Integrated Development Environments which will be covered in this report are the following:
+ Breakpoints
+ Output Console
+ Diagnostics
+ Variable changing
+ Call stack viewing

## Debugging

### What is debugging?
Debugging is the process of identifying and solving defects or issues within an application so that it works as intended. It is mostly used within the development and testing phases of application development.

The debugging process normally consists of a few steps, the following are the four main steps involved:
+ Identifying a bug
+ Classifying a bug
+ Understanding a bug
+ Repairing a bug

### Debugging process
The aforementioned four steps of the debugging process are the following:

#### Identifying a bug
The source of the problem is located within the code during this step. Depending on the size of the code and the experience of the programmer, this can prove to be one of the harder parts of debugging. This is because an inexperienced programmer may be confident with their code, believing it works – until it doesn’t. As a result, a large amount of code may have to be checked to find the problem. If the debugger outputs a message pointing to the potential location of the problem, it must be analysed to see whether this is the source of the problem or if there may be further issues elsewhere. If the debugger does not output the location of the bug, the whole code must be checked according to the error message.

#### Classifying a bug
In this step, the previously located bug must be classified so that it can be solved accordingly. There are four different types of bugs which may occur:

+ Syntactical Errors - These types of errors will usually be found by the compiler. However, just because the error has been found by the compiler does not mean the error message will always be accurate to the location of the bug.

+ Build Errors - This type of error will happen when files which have been linked within code have not been rebuilt after changing their source code, causing them to not work.

+ Basic Semantic Errors - These errors occur when there are unused variables or blocks of code or issues with the variable types being used. 

+ Semantic Errors - This type of error occurs when the wrong variables or operators are used. This type of error can’t be picked up by any tools, due to the code being syntactically correct but logically wrong. They can only be spotted by using a test case or a debugger.

#### Understanding a bug
Before any repairs are attempted, the bug should first be fully understood. Attempting repairs to a bug which is not understood may cause further problems in the code. This is because the problem may change forms and change to another location unpredictably.

There are a couple of things which can be done during this step in order to understand the bug:
+ Do not mix symptoms with the real cause of the problem
+ Check other parts of the code for similar problems
+ Be sure that the problem is a programming bug and not an issue with the code on a fundamental level

#### Repairing a bug
The final step of the debugging process is the repair. There is more to this step than just fixing the issue, it must be documented and tested thoroughly. This is because doing so will allow for future bugs to be solved more effectively; such as spotting a pattern in the causes of problems, allowing for adaptation to the code to avoid that problem altogether. Filing in a document explaining the process used to solve a bug can be a useful practise.

Several points about the debugging process are worth noting:

+ How the bug was first noticed.
+ How the bug was narrowed down to the exact cause.
+ What the bug can be classified as.
+ How often the bug occurred.
+ If initial assumptions were incorrect.


## Debugging Facilities

### Breakpoints

### Output Console

### Diagnostics

### Variable changing

### Call stack viewing

## Building a Robust Application

## Conclusion

## References
***Adragna, P. (2008). Software debugging techniques - CERN Document Server [online]. Available at: https://cds.cern.ch/record/1100526/files/p71.pdf [Accessed 28 Nov. 2018].***   
***Itu.dk. (1979). Debugging Techniques. [online] Available at: http://www.itu.dk/~slauesen/Papers/DebuggingTechniques.pdf [Accessed 30 Nov. 2018].***   
