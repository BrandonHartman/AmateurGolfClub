Problem Definition
----------------------------------------

The Springfork Amateur Gold Club has a tournament every weekend. The club president has asked you to write a program that reads names of golfers and their scores using keyboard input and then prints a report. You will write a Python program that saves all the input to a file and then reads the file to output the report. 

The program will have three functions that do the following: A main() function that simply calls the other two functions. That is to say the main( ) function will simply perform the following calls: Call input golfer’s information. 2. Call display golfer’s tournament report. An inputInfo() function has a loop. Inside the loop are statements to input golfer name and score for one golfer and write them to file. Make sure to validate input. The loop repeats to read multiple golfer information until a user enters ‘n’ in response to: “Do you have more golfers to enter? (y/n).” 

Here is the algorithmic flow of the statements: 1. Open “golf.txt” file for writing 2. Display “Are there any golfer cards to input? (y/n) “3. Read response from keyboard 4. Repeat until response is not equal to ‘n’. A. Read golfer name from the keyboard. B. Read golfer score from the keyboard. C. Write golfer name and score to file. D. Display “Do you have more golfers to enter? (y/n)” E. Read response from keyboard. 5. Close file. A displayReport() function opens the “golf.txt” file and reads all golfers and their information one at a time in a loop and displays each golfer as a row in a table to the screen. 

Analysis
----------------------------------------

We have picked Python as our language for this project because we are currently learning the programming language in class. The program will head into the main() section that will host the other two sections that develop the program as needed. The other sections will be named inputInfo() and displayReport() and these sections will hold the content that must be applied to create the program project. However, the program will not until the main() is called in the program. Once called into play, the main will call onto the inputInfo() to get the users information as needed. Afterwards, it will call onto the displayReport() to display the outcome of the project that must be acquired. 

Heading into the inputInfo() once main is called within the project. The program will start by opening the ‘golf.txt. file within the computers documents to write onto it. However, it must be handled with cation because it will overwrite data. The program will call and open the file and choose ‘w’ to write onto the file. Afterwards, the program will set a variable named userResponse. This will be used to receive input from the user. The input will ask the user if there are any golfer cards to input. It will also ask for an input of ‘y’ for yes or ‘n’ for no. If selected ‘y’, it will process into a while loop. If selected ‘n’, it will display a ‘Thank you for playing’ message and will close the application. If user inputs something that is invalid for the program. It will display an invalid input message and tells the user to please try again later. The application will close afterwards. Heading into the while loop, this will state that the users input is equal to ‘y’ and will lead into the next segment of the program. The program will process into the next part by asking the user to input the name of the golfer that is playing. This input will be assigned to the variable known as golferName.

 After golferName is assigned, the program will go into the project file to write the golferName variable onto the text within the computer. The name will also contain a newline function after golferName is set and declared. The program will process into the next part of the while loop. The program will ask the user to input a score that was tallied while playing the game. This input will be assigned to the variable name known as golferScore. After golferScore is assigned, the project will go into the project file to write the golferScore variable onto the text within the computer. The name will also contain a newline function after golferScore is set and declared. The program will proceed into the final part of the loop. It will ask the user if there are any more golfers to enter into the program. Again, ‘y’ for yes or ‘n’ for no. The loop will end and procced down the list to the next line of programming code. Next in line states that the .close() function will close any file that was recently opened for any reason. This will close the project file to until it is called to open again.

After inputInfo() is closed,  main() will call onto the displayReport() to display the information gathered by the user. Heading into the displayReport() once the main calls it. The program will start to open the ‘golf.txt’ file inside the computer to read within it. The program uses the open function to read the information from the file. The program uses ‘r’ to do so.  The program will proceed through the code and will assign zero to the variable named bestScore. This will be achievable once the program is completely finished and calls the variable to state what score won at the end of the visual display on the screen. Moving into the next section, the program will assign none to the variable named winnerOfGame. This will be set in a if statement later processed within the code. However, at the moment it will be set to none until it is passed into becoming something.

 Leading into the next section, will state that it is reading the input that the user typed for golferName and will be finished once the line is read from the project file. Before entering into another while loop. The code will produce four print statements onto the screen stating what the club is, the tournament date and where the name and scores go after being aligned. These print statements will formatted and aligned if needed. Afterwards, it will procced into a while loop that states while golferName is not equal to an empty string that it will process into a loop to gather information.  It will lead into a state that is reading the input that the user typed for golferScore and will be finished once the line is read from the project file. This will be converted into an integer by using the int function. 

This will lead into the next process of the while loop as golferName will be printed fir display and formatted to the aligned area that must be done. The program uses the .rstrip() function to strip the newline away from golferName. It will be aligned thirty-nine characters to the right.  Heading into the format of golferScore. It will state that golferScore is also getting printed for display and formatted as needed. golferScore will be formatted fourteen character spaces to the left and assigned as an integer. So it will need be formatted with ‘d’. When the formatting and display is finished; the program will run into a if statement that will process through if golferScore is less than or equal to bestScore. Earlier in the program, bestScore is set to 0. So if the user puts anything that continues as positive. It will run the if statement.

Once inside the if statement, bestScore will be assigned to the variable to the variable defined before known as golferScore. After assigning the bestScore; the program needs to assign who wins the game of golf. The program will assign the winnerOfGame to the variable known as golferName. The same variable that was assainged before. Afterwards, a line of code will state that it is reading the input that the user typed for golferName and will be finished once the line is read from the project file. Once the file is read, the program will display the winner of the game and score. Calling the two assigned variables from winnerOfGame and bestScore. Afterwards, the program will no longer need the project files. So the program will need to use the .close() function to close the file until the being called again by the open() function. 


Design
-------------------------------------------

Here is the Pseudocode: ------------------------------------------------------------------------
•	Define the main
o	Define inputInfo and what is inside of it
o	Define displayReport and what is inside of it
•	Call main so that it goes into inputInfo and displayReport
•	---------------------------------------------------------------------------------------------
•	Inside inputInfo
o	Open golf.txt to write data onto it
♣	Attain input “Are there any golfers to input? (y/n)
♣	Assign that to the variable userResponse
♣	Head into a while loop. While userResponse equals ‘y’
♣	Attain input “Enter a name of the golfer”
o	Assign that to the variable golferName
♣	Write the golferName into the project file
♣	Adding a newline with it
♣	Attain input “Enter the score of the golfer”
o	Asign that to the variable golferScore
♣	Write the golferScore into the project file
♣	Adding a newline to it
♣	End the loop by asking for any more golfers
o	Assign the input to userResponse
♣	If userResponse equals to ‘n’
♣	Display “Thank you for playing. Have a wonderful day!”

♣	Else for any invalid input
♣	Display “Invalid input. Please try again later. Goodbye!”
o	Close the file that was written on.

•	-----------------------------------------------------------------------------------------------
•	Inside displayReport
o	Open golf.txt to read within it
♣	Create a variable named bestScore
♣	Assign it to zero
♣	Create a variable named winnerOfGame
♣	Assign it to none
♣	Read the input the user typed for golferName
♣	Display “SPRINGFORK AMATEUR GOLD CLUB”
♣	Format is as a string and thirty-nine spaces to the right
♣	Display “TOURNAMENT: WEEKEND OF NOVEMBER 4th”
♣	Display “GOLFER NAME                                        SCORE”
♣	Display “-------------------------------------              --------------
♣	Process into a while loop: golferName is not equal to empty string
♣	Read the input the user typed for golferScore
o	Along with a int function
♣	Display golferName
o	Format thirty-nine spaces to the right with ‘s’
o	Strip the newline
♣	Display golferScore
o	Format fourteen spaces to the left
♣	If golferScore is greater than best score
o	bestScore will equal golferScore
o	winnerOfGame will equal golferName
♣	Read the golferName variable within the project file
♣	Display “The winner is”, WinnerOfGame, “With score”, bestScore
♣	Close project file using the close function
♣	Celebrate that project is finished 

Implementation
------------------------------------------------
The development environment used for this program was PyCharm CE. I programmed it on my Mac pro using the OS Operating System. I had a couple unusual situations happen while developing this program. The main concerns for this program would have been the formatting within the program. Just to state exactly what the professor wanted. I would fix this problem by lowering the counted spaces and read within the function of readline() instead of read.
