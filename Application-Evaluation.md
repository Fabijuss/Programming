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

     // Stores the current mouse position  
		function MousePos (event) {
			var bounds = canvas.getBoundingClientRect();
		
			mouseX = event.clientX - bounds.left
			mouseY = event.clientY - bounds.top
			
		}
		
		// Checks players position and sets inside canvas bounds		
		function CheckBounds ()
		{
			if (playerPosX < 0) {
				playerPosX = 0
			}
			
			if (playerPosY < 0) {
				playerPosY = 0
			}
			
			if (playerPosX > canvas.width) {
				playerPosX = canvas.width
			}
			
			if (playerPosY > canvas.height) {
				playerPosY = canvas.height
			}
		}
	
		
		//calculates distance from enemy to player 
		function calcAngle ()
		{
			var differenceX = playerPosX - enemyX
			var differenceY = playerPosY - enemyY
			
			var angle = Math.atan2(differenceY, differenceX)
			
			enemyX += speed * Math.cos(angle)
			enemyY += speed * Math.sin(angle)
		}
	
		//refreshes canvas to update player and enemy position
		//invulnerability time if player recently touched enemy
		function GameLoop () {
			playerPosX = mouseX
			playerPosY = mouseY
	
			CheckBounds()
			calcAngle()
			
			
		
			if (iframeCounter == 0) {
				if (playerPosX < enemyX + enemySize && playerPosX + playerSize > enemyX && playerPosY < enemyY + enemySize && playerPosY + playerSize > enemyY) {
					iframeCounter = 60
					lives -= 1
					document.getElementById("counter").innerHTML -= 1;
				}
			} else {
				iframeCounter -= 1
			}
			
			
			// Reset everything when lives reaches 0
			if (lives <= 0) {
				playerSize = 50
				enemySize = 50
				iframeCounter = 0
				playerPosX = 0
				playerPosY = 0
				enemyX = canvas.width
				enemyY = canvas.height
				speed = 10
				lives = 3
				document.getElementById("counter").innerHTML = "3";
			}
			
			//colour of player & enemy
		    context.fillStyle = '#f7f7f7';
            context.fillRect(0, 0, canvas.width, canvas.height);
			context.shadowColor = 'black';
			context.shadowBlur = 5;
			
			
			context.fillStyle = "#686868";
			context.fillRect(enemyX-(enemySize/2), enemyY-(enemySize/2), enemySize, enemySize);
			
			// iframe colour
			context.fillStyle = "#a5a5a5";
			if (iframeCounter > 0) {
				context.fillStyle = "#e0e0e0";
			} else {
				context.fillStyle = "#a5a5a5";
			}
		
			context.fillRect(playerPosX-(playerSize/2), playerPosY-(playerSize/2), playerSize, playerSize); 
			
			window.requestAnimationFrame(GameLoop)
		}
	  
		// Program starts here
		var canvas = document.getElementById('game-canvas'); 
		var context = canvas.getContext('2d');
		var speed = 10	
		
		var lives = 3
			
		var playerSize = 50
		var enemySize = 50
		
		var iframeCounter = 0
		
		canvas.width = 800
		canvas.height = 600
		
		var enemyX = canvas.width
		var enemyY = canvas.height
		var playerPosX = 0
		var playerPosY = 0
		
		var mouseX = -100
		var mouseY = -100
		
		// Lives counter
		document.getElementById("counter").innerHTML = "3";
		
		window.addEventListener ("mousemove", MousePos)
		window.requestAnimationFrame(GameLoop)
 
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




