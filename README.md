# Intergration-Project
#Allison Schwarz
#Taylor Swift song quiz game

def playerinfo():                   #function definition
    playerName = input("Enter your name: ")
    print("Hello " + playerName + "! Let's get started!")
def main():
    print("Welcome to my Taylor Swift trivia game!")  # greeting
    playerinfo()
main()

score = 0

question1 = "How many studio albums has Taylor Swift released?: \n\n"  #questions
question2 = "What type of music does Taylor Swift sing?: \n\n"
question3 = "What year did Taylor Swift release her debut(first) album?: \n\n"
question4 = "How many grammy's has Taylor Swift won?: \n\n"
question5 = "When is Taylor Swift's next album being released?: \n\n"

options1 = "A: 8\n" "B: 9\n" "C: 11\n" "D: 7\n\n"
options2 = "A: country\nB: pop\nC: indie/folk\nD: all of the above\n\n "  #answers
options3 = "A: 2003\nB: 2007\nC: 2006\nD: 2005\n\n"
options4 = "A: 5\nB: 9\nC: 13\nD: 11\n\n"
options5 = "A: November 13th, 2022\nB: October 21st, 2022\nC: December 1st, 2022\nD: October 7th, 2022\n\n"

correct1 = "B"          #correct answers
correct2 = "D"
correct3 = "C"
correct4 = "D"
correct5 = "B"

print(question1 + options1)  #string operator to print 2 variables

answer1 = input("Enter A, B, C, or D: ")
def check_ans(question1):
    if answer1 == correct1:   #used relational operator ==
        print("Correct!\n\n")
        return True
        score += 1                #used the shortcut operator +=
    else:
        print("Incorrect!\n\n")
        return False
check_ans(question1)

print(question2 + options2)

answer2 = input("Enter A, B, C, or D: ")
def check_ans(question2):        #function definition
    if answer2 == correct2:
        print("Correct!\n\n")
        return True
        score += 1                #used the shortcut operator +=
    else:
        print("Incorrect!\n\n")
        return False
check_ans(question2)
print(question3 + options3)

answer3 = input("Enter A, B, C, or D:")

if answer3 == correct3:
    print("Correct!\n\n")
    score += 1
if answer3 != correct3:        #used the relational operator !=
    print("incorrect!\n\n")

print(question4 + options4)

answer4 = input("Enter A, B, C, or D:")

if answer4 == correct4:                #used the standard conditional structure if
    print("Correct!\n\n")
    score += 1
else:                                  #used the standard conditional structure else
    print("incorrect!\n\n")

print(question5 + options5)

answer5 = input("Enter A, B, C, or D:")

if answer5 == correct5:
    print("Correct!\n\n")
    score += 1
if answer5 != correct5:        #used the Boolean operator !=
    print("incorrect!\n\n")

totalscore = str(score / 5 * 100)       #used / to divide the score by five and * to multiply by 100
def playerscore():
    print("You got " + str(score) + " questions correct!")   #function that accepts parameters
    print("You got " + totalscore + "%. ")
def main():
    if totalscore == 100:
        print("Congratulations! You got a perfect score!")
    elif totalscore == 80:      # if/elif/else statement
        print("Good job! You did well!")
    elif totalscore == 60:
        print("Pretty good!")
    elif totalscore == 40:
        print("Go listen to Taylor Swift")
    else:
        print("Go stream Taylor Swift")
    playerscore()
main()

if totalscore > str(50) and totalscore< str(100):     # used the Boolean operator and
    print("You passed!")
if not totalscore >str(50):             #used the Boolean operator not
    print("You failed :(")
if totalscore > str(100) or totalscore== str(100):    #used the Boolean operator or
    print("You got a perfect score!")

num=0
while (num<1):                     # used the while standard iterative structures
    num = num + 1
    print("Thank you for playing my game!")


#This is the end of my program, but here are examples of some of the project requirements I could not include naturally:
    #Modulus works like this: 4%3 = 1
    #Exponentation works like this: 2**3 = 8
    #Floor division works like this: 5//2 = 2
    #Addition works like this: 2+2 = 4
    #Subtraction works like this: 5-3 = 2
    #range(), for, and in works like this:
for i in range(4):
    print(i, end=" ")
print()
