This project is made by:
    Amanvir Singh
    2310740

    Jasmeet Kaur
    2310337

    Manvir Kaur
    2310376



This is a Python based Python Learning Program. in which the user has to read the module at every level and have to pass a quiz
related to the module he has read. He has to obtain a certain percentage in the quiz to move to the next level. After all the levels,
the user has to pass the final quiz which contains questions based on all the modules. For now, there are only 2 basic levels and one
final level but we can add more levels to it just by introducing slight modifications. The program has a sign up and sign in option to
track the performance of every user. The user can reset his course after completion and he can also change the password for his username.
The program, can only be run by 'Main' file, if someone accesses through other files, the program terminates. The program also has a captcha
feature to verify a human while signing up and logging in. It also verifies the style of email address(like does it contain @, etc.). It also 
has Secured Entry for password which will not show password on terminal while typing. There are special admin login credentials which can be
used to view details of users, view quizzes, etc. We implemented the program such that we can update the Question bank anytime and the program
will reflect changes automatically, like it will pick certain amount of random questions from that question bank.


ADMIN PANEL LOGIN DETAILS:
Username: adminajm
Password: qwerty
or
Username: computer
Password: 010101

BRIEF DESCRIPTION OF EVERY FILE:
TXT Files: The files with 'level' as prefix are the modules the user has to read, these files will be printed on terminal. The number represents
the level of module while '-1' represents final module
The files with 'quiz' as prefix are the question banks for the each module. At beginning of these files, there are answers to questions stored
in dictiionary

Main.py : This is the main file which hadles almost everything. The program should be run by executing the main file. This file calls the
functions respectively. It shows the user a menu after they logged in to choose from. It has the level increase function which increases
level everytime user passes a quiz. It opens all the modules to read. This file also has the update password function to change password. 
It also has functions for Opening the source code on github and repltit directly.

Login.py: This file is responsible for sign up and login whether as a student or as an admin. It validiates every detail enterd by user while 
signing up. This file conatins the captcha function. It also stores the user information in CSV file. This file also checks for admin logins.
All in one, it takes care of signing options

Quiz_main.py: This file is responsible for the quizzes. It goes through the quiz file, picks up the random question, displays it and ask user
for their answer. It then checks the answer, stores the marks and move on to next random question in the file. This file is made in a way that
it will ask the user 3/4 of the questions present in the question bank which will reflect random questions on screen. It also calculates
the final marks and return the result to the main file.

Login Details.csv : This file as the name suggests, stores the user information in CSV format. It contains login details of every student but
not the admin(For admin, that are stored in login.py file itself). 

