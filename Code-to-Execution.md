# Code to Execution 
#### Outlining the Steps Taken from Writing Code to Execution.
## Contents
[I. Contents](#contents)   
[II. Introduction](#introduction)   
[III. Interpretation](#interpretation)   
&nbsp;&nbsp; [III.1. Coding](#coding)   
&nbsp;&nbsp; [III.2. Interpreting](#interpreting)   
[IV. Compilation](#introduction)   
&nbsp;&nbsp; [IV.1. Coding](#coding)   
&nbsp;&nbsp; [IV.2. Compiling](#compiling)   
&nbsp;&nbsp; [IV.3. Assembly](#assembly)   
&nbsp;&nbsp; [IV.4. Linking](#linking)   
&nbsp;&nbsp; [IV.5. Execution](#execution)   
[V. Conclusion](#conclusion)   
[VI. References/Bibliography](#references)   

## Introduction
This report will cover the steps taken from writing the code, to the execution of the code. This report will be split into two main sections, one for each type of code execution. The two ways that code can be executed, are by interpretation and by compilation. 

## Interpretation
This method of executing code, is best suited for procedural paradigm applications. This is because interpretation reads and executes each line of code individually. This means that any errors in the application will be ignored until the interpreter gets to the line of code that causes issues and stops executing.  
Some examples of interpreted languages include: Java, Python, Ruby, PHP.
Interoperation involves the following steps:

### Coding
This is the phase where the application source code is written. This phase includes multiple changes to the source code, ranging from adding new features to general debugging. This process is generally aided by the use of an IDE, which can include automated diagnostic and debugging tools. 

### Interpreting 
The process of interpretation is carried out by an interpreter. An interpreter is a high-level programming language translator that allows the machine to understand the programming used. The way an interpreter works is by reading one line of code, translating it into machine code, and then executing it. This process is done for every single line of code, so long as there are no errors that the interpreter cannot translate. Interpreted programs stay in the source language used to create the program, unlike compilation which turns the program into assembly. 

## Compilation
This method of executing code results in an executable file which can be installed on different computers. Running the application will execute the machine code instructions located in the executable file. Compilation will not work If there are issues which cannot be translated in the compilation process. 
Some examples of languages that use compilation include: C, C++, C#.
Compilation involves the following steps:

###Coding
This is the phase where the application source code is written. This phase includes multiple changes to the source code, ranging from adding new features to general debugging. This process is generally aided by the use of an IDE, which can include automated diagnostic and debugging tools. 

### Compiling
The process of compilation involves taking the source code and translating it into machine code with the use of a compiler. This process will check the source code for any errors, and will abort the process if any errors are detected preventing it from being translated. This will end up generating assembler source code.

### Assembly
This is a stage after compiling which is the next step of the compilation process. The assembly source code is taken and an assembly listing is produced.  The output from the assembler is stored in an object file.

### Linking
This is the final stage of the compilation process. In this step, the object files and libraries are taken as input and combined to form an executable file. This results in a file which has properly referenced external symbols with assigned final addresses to functions and variables.

### Execution 
The application can be started by launching the executable file, which loads the program’s machine code instructions into the CPU. This will allow the program to run until it is terminated either by the normal means, or through an unexpected event such as a crash.

## Conclusion
To conclude, interpretation and compilation are similar yet two different ways of executing an application. They are best suited to specific languages which are built around that type of application execution. Interpreter is ideal for applications that do not require all of the code to be used at any given time, and instead to be used in a procedural manner such as a command-line application. Meanwhile, compilation is best used for applications that require all of the files to be linked and the code to be read at any given place. For example, in a game application.

## References
Www2.hawaii.edu. (n.d.). The Programming Process. [online] Available at: http://www2.hawaii.edu/~takebaya/ics111/process_of_programming/process_of_programming.html [Accessed 6 Dec. 2018].



