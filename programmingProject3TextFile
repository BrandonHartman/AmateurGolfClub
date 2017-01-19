# -----------------------------------------------------------------------------
# Programming Project Three
# Brandon Hartman
# November 4th, 2016
# -----------------------------------------------------------------------------

# The Springfork Amateur Gold Club has a tournament every weekend. The club president has
# asked you to write a program that reads names of golfers and their scores using keyboard input
# and then prints a report. You will write a Python program that saves all the input to a file and
# then reads the file to output the report.

# This program will host three different types of sections. Main(), displayingReport()
# and inputInfo(). The main() function will be the one that calls the other two into the program
# However, the program will not work until the main function is called. Once called into play..
# The main will call onto the inputInfo() to get information. Afterwards, it will call onto
# the displayReport() to display the outcome of the project that we are looking at.


def main():
    # This is the definition of the main function.
    inputInfo()
    # The function gathers input information from the user once main() is called at the end.
    displayReport()
    # This function displays the report that the last function inputInfo() acquired and processes
    # the information through statements and loops.


def displayReport():
    # Heading into the displayReport() once the main is called. The program will start to open the
    # 'golf.txt file inside the computer to read within it. The program uses the open function to
    # read the information from the file. The program uses 'r' to do so.
    programProjectFile = open('golf.txt', 'r')
    # The program assigns zero to the variable named bestScore. This will be achievable once the
    # program is completely finished and calls the variable to state what score won at the
    # end of the visual display on the screen.
    bestScore = 0
    # The program assigns none to the variable named winnerOfGame. This will be set in a if statement
    # later processed within the program. However, at the moment..It will be None until it is passed
    # into another variable.
    winnerOfGame = None
    # This states that it is reading the input that the user typed for golferName and will be
    # finished once the line is read from the project file.
    golferName = programProjectFile.readline()
    # This will display the title of the program. This states that it is formatted as a string
    # thirty-nine spaces to the right.
    print(format("SPRINGFORK AMATEUR GOLD CLUB", '>39s'))
    # This is the second section of displayed program. This states the tournament weekend.
    print("TOURNAMENT: WEEKEND OF NOVEMBER 4th - 04 NOVEMBER 2016 ")
    # The last section of simply using the print function of the display area without input.
    # This will display the section area for golfer name and score.
    print("GOLFER NAME                                      SCORE")
    # A breaking point within the printing functions. To add a design to break the sections
    # apart.
    print("---------------------------------------          -----")
    # This states that while golferName is not equal to an empty string that it will
    # process into a loop to gather information.
    while golferName != '':
        # This states that it is reading the input that the user typed for golferScore and will be
        # finished once the line is read from the project file. This will be converted into
        # a integer by using the int function.
        golferScore = int(programProjectFile.readline())
        # This leads into the next process of the while loop as golferName will be printed for
        # display and formatted to the aligned area that must be done. The program uses the .rstrip()
        # to strip the newline away from golferName. It will be aligned thirty-nine characters to the
        # right.
        print(format(golferName.rstrip(), "<39s"),
              # This states that golferScore is also getting printed for display and formatted as needed.
              # golferScore will be formatted fourteen character spaces to the left and assigned
              # as an integer. So it will need to be considered for format 'd'.
              format(golferScore, ">14d"))
        # The program will run into a if statement that will process through if golferScore is less than
        # or equal to bestScore. Earlier in the program, bestScore is set to 0. So if the user puts anything
        # that continues as positive..It will run the if statement.
        if golferScore >= bestScore:
            # Once inside the if statement, bestScore will be assigned to the variable defined before known
            # as golferScore.
            bestScore = golferScore
            # After assigning the bestScore...The program needs to assign who wins the game of golf.
            # The program will assign the winnerOfGame to the variable known as golferName. The
            # same variable that was assigned before.
            winnerOfGame = golferName
        # This states that it is reading the input that the user typed for golferName and will be
        # finished once the line is read from the project file.
        golferName = programProjectFile.readline()
        # This will display the winner of the game. THis will be print "The winner is" and call the
        # variable winnerOfGame and to be printed on the screen.
    print("The Winner is", winnerOfGame)
    # Afterwards, the program will no longer need the project files. So the program will
    # need to use the .close() function to close the file until being called again by the
    # open() function.
    programProjectFile.close()


def inputInfo():
    # Heading into the inputInfo() once main is called. The program will start to open the
    # golf.txt file inside the computer to write onto it. However, it must be handled
    # with cation because it will overwrite data. We will call and open this file and
    # choose 'w' to write onto the file.
    programProjectFile = open('golf.txt', 'w')
    # Afterwards, setting a variable named userResponse. This will be used to receive
    # input from the user. The input will ask if there are any golfer cards to input.
    # It will also ask for an input of 'y' for yes and 'n' for no. If selected 'y'..
    # it will go into a while loop. If selected 'n'. It will display a thank you for playing
    # message and close the application. If user inputs invalid input.. It will display a
    # invalid message and to try again later. The application will close as well.
    userResponse = input("Are there any golfer cards to input? (y/n) ")
    # Heading into the while loop. This will state that if the users input is equal to
    # 'y' that will function into the next segment of the program.
    while userResponse == "y":
        # The program will process into the next part of the loop. It will ask for the
        # user to input a name of the golfer that is playing. This input will be assigned
        # to the variable known as golferName.
        golferName = input("Enter the name of the golfer! ")
        # After golferName input..The program will go into the project file to write
        # the golferName variable onto the text within the computer. The name will also
        # contain a newline function after golferName is set and called.
        programProjectFile.write(golferName + '\n')
        # The program will process into the next part of the loop. It will ask for the
        # user to input a score that was tallied during the game. This input will be assigned
        # to the variable name known as golferScore.
        golferScore = input("Enter the score of the golfer! ")
        # After golferScore input.. The project will go into the project file to write
        # the golferScore variable onto the text within the computer. The name will also
        # contain a newline function after golferScore is set and called.
        programProjectFile.write(golferScore + '\n')
        # The program will process into the final part of the loop. It will ask the user if there
        # are any more golfers to enter into the program. 'y' for yes and 'n' for no.
        userResponse = input("Do you have more golfers to enter? (y/n) ")
    # This statement state that if the user enters 'n' for userResponse that the application
    # will display a thank you message on the screen and close.
    if userResponse == 'n':
        print("Thank you for playing. Have a wonderful day!")
    # This statement states anything other than 'y' and 'n' will be invalid. Else, states that
    # it will print a invalid input was entered and to try again later. The application will
    # close.
    else:
        print("Invalid input. Please try again later. Goodbye!")
    # This states that the .close() function will close any file that was recently opened for
    # any reason. This will close the project file until called to open again.
    programProjectFile.close()
# This states that the main function is being called and will run whatever is in the main function.
main()
