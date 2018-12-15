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
&nbsp;&nbsp;[V.1 Robustness](#robustness)   
&nbsp;&nbsp;[V.2 Security](#security)   
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
Integrated Development Environments (IDEs) often come with a number of different debugging facilities in order to aid with programming. Most IDEs have the same few facilities which give most of the basic and needed tools for debugging. However, some IDEs come with different sets of tools to aid with particular problems or programming languages. 
The following are some of the main debugging facilities available in IDEs;

### Breakpoints
This debugging tool allows the code to have set points in which the application stops. The main usage of this tool is to allow the programmer to inspect the values that certain variables have at certain points in the application, to ensure that they are as intended. This is important to ensure that issues do not arise in the future, as the application may work with incorrect values but the outcome could produce errors or unexpected results.

### Output Console
This tool is used to output certain information into a console. The console usually reports any errors which are picked up while the application is running. It is possible to attach the console to certain parts of the code, allowing for uses such as outputting the variables into the console so that they can be inspected. The console can also be a useful tool when checking if everything works as intended. For example, it can be used to check if a script file has been loaded correctly, by seeing if any errors occurred in the console while loading the script.  

### Diagnostics
This is a tool used to assist in troubleshooting issues such as memory leaks, memory fragmentation, crashes, slow performance and hangs. This tool analyses the code of the application by using built-in rules from various applications and Microsoft technologies. Once it analyses, any detected problems are outlined so that they may be fixed. The diagnostics tool can be useful when there are various performance issues with the application, but the source of the problem is not clear. It can also be useful when there is a lot of code or when the code is complex, which may cause the problem to not be apparent. 

### Variable changing
This tool is used to change variable in the code during runtime. This can be done by using the aforementioned breakpoints in order to stop code in certain parts, and then changing the variables in order to test different outcomes. This can be useful to test what kind of values can cause errors in the application, so that the code does not accept them. It can also be used to test input variables quickly, without having to run the code every time to see each input’s outcome.

### Call stack viewing

This tool is used to see what functions are called at certain points in the program. As with variable changing, this tool utilises breakpoints in order to see what functions have been called at certain points in the program. This tool can be useful when checking if functions have been called correctly and in the right order. Furthermore, it can be used to check the values which are currently being used in the functions. This can be very important as a function relying on certain values may break the entire code if the values are incorrect. 
## Building a Robust Application
While debugging is primarily used in order to solve problems to ensure an application works as intended, it does come with the added benefit of improving security by patching holes in the application. Furthermore, solving issues with the application can prevent problems such as crashing or unexpected errors, thus increasing the overall robustness of the application.

### Robustness
The primary usage of debugging is to iron out issues so that an application works properly, robustness directly ties in with this as the more issues are solved, the less likely further issues are to arise. For example, if the application has issues with certain inputs from the user, if the allowed inputs are limited to only ones that are acceptable for the application, then the chances of an issue caused by inputs is greatly reduced.

The process of debugging can reveal many issues within the code of the application, this allows the programmer to find the most vulnerable spots and reinforce them by using different logic, limiting certain factors and rearranging the code in order to prevent issues before they appear. Furthermore, it allows the application to feature certain fail-safes in the case of an unexpected error, such as setting the code back to a certain point 

### Security
The security and the robustness of an application are directly correlated, as an application which cannot perform unpredictably will have few vulnerabilities which can be exploited. There are many applications which use sensitive data, which would cause severe damage if they were leaked. Thus, debugging is used to locate and remove any bugs that may be causing vulnerabilities in the code, to ensure that they cannot be exploited.

During the debugging process, certain vulnerabilities will arise, these include inputs, encryption of data, certain values in variables and various other vulnerabilities. It is vital that they are addressed during this phase as leaving them in the code is a sure-fire way of compromising the security of the application. Fully understanding the vulnerabilities in the code allow for countermeasures to be put into place, such as deleting data if the security is compromised, or shutting the system off if a irregularity is detected.  

## Conclusion
To conclude, it can be seen that debugging is a vital step in the development process of an application, as without the application is likely to suffer in terms of security and reliability. Being able to identify, understand and repair a bug is essential in order to first troubleshoot the issue, as well as being able to prevent it from further arising in the future. 

Furthermore, the debugging process highlights vulnerabilities in the structure and logic of the code, patching these vulnerabilities increases both the robustness and security of an application, which is critical in applications that handle sensitive data, and in any applications that require 100% up-time. 


## References
***Adragna, P. (2008). Software debugging techniques - CERN Document Server [online]. Available at: https://cds.cern.ch/record/1100526/files/p71.pdf [Accessed 28 Nov. 2018].***   
***Itu.dk. (1979). Debugging Techniques. [online] Available at: http://www.itu.dk/~slauesen/Papers/DebuggingTechniques.pdf [Accessed 30 Nov. 2018].***   
