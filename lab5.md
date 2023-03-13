## Lab report 5
The favourite lab I decided to choose is lab 3 where we need to utilize the grep, I will explore different commands than ones I used in lab 3

** The first command I'd like to explore is grep -i:
* This command makes the argument not case sensitive, meaning the upper case and lower case doesn't matter here. 
* When I inputed grep -r -c "School", the result is the following:
* <img width="625" alt="image" src="https://user-images.githubusercontent.com/103611867/224823042-2a2aefcf-7147-4a8a-b4a1-1b0efb178884.png">
* However when I change the command to grep -r -c -i "School", the number of counts increased:
* Output: <img width="596" alt="image" src="https://user-images.githubusercontent.com/103611867/224822958-3b212789-b702-4183-ada8-c68e323791cf.png">
* It makes sense because now we "igores" uppercases, but consider all words that matches "school"
* Source: https://ryanstutorials.net/linuxtutorial/cheatsheetgrep.php


** The second command I would like to explore is egrep -n 'String' [file name]
* This command will print out each line that contains the keyword I specified, as well as show the line, without -n it won't show which line it is in the file 
* Like when I enter the command egrep -n 'School' PuertoRico-WhatToDo.txt, it will give me the following output:
* Output: <img width="904" alt="image" src="https://user-images.githubusercontent.com/103611867/224825163-ef4ead66-12e3-4aef-9deb-b67fb8422025.png">
* Source: https://ryanstutorials.net/linuxtutorial/cheatsheetgrep.php

** The third command I would like to explore is find -empty:
* This will give us the empty file and folder
* output: <img width="458" alt="image" src="https://user-images.githubusercontent.com/103611867/224843343-b8ec3401-328e-4a4f-9a7c-e9feb3fe651f.png">
* This gives me empty folders which are branches, tags, and info. 
* Source: https://www.geeksforgeeks.org/find-command-in-linux-with-examples/




