# comp206---structure-and-csv-files-in-c-solved
**TO GET THIS SOLUTION VISIT:** [COMP206 – Structure and CSV Files in C Solved](https://www.ankitcodinghub.com/product/comp206-structure-and-csv-files-in-c-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;110739&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP206 - Structure and CSV Files in C Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Labs F, G and lecture 20 will provide some background help for this mini assignment.

QUESTION

Write a C program called: ./database CMD OPT1 OPT2 OPT3 OPT4 Where:

• CMD is a command that performs a specific operation.

• OPTi are optional arguments depending on CMD.

The source file is called: database.c

The executable file is called: database

The CSV file is called: database.csv

The argument CMD can have the following values:

• SHOW – displays all the records from the database.

• DELETE – OPT1 = ID, that record in removed from the database.

• ADD – OPT1=ID, OPT2=NAME, OPT3=AGE, OPT4=GPA, a new record with these fields are added to the database.

The structure of the CSV file is: ID,NAME,AGE,GPA

Spaces can exist between the commas, but are not required. In other words, your program should handle both cases. If a space comes after or before a comma, then it is not considered to be part of the field.

For example, database.csv could look like this:

10,bob,18,3.5

15,mary,20,4.0

5,tom, 17 , 3.8

Notice the record “tom” has spaces before and after some of the commas. These spaces are not part of the fields. In other words we read: “5” then “tom” then “17” then “3.8”, without spaces in the field characters.

Create database.csv and database.c in the same directory. Using vim, initialize database.csv with the above three records (i.e. bob, mary, tom), with the same spacing and format.

Make database.c do the following:

1. If the user does not provide any command line arguments, then terminate with an error message: “Your did not provide any arguments. Please enter: ./database CMD OPT1 OPT2 OPT3 OPT4”.

2. If the CMD argument is not SHOW, not DELETE, not ADD, then terminate the program with the error message: “The command you requested in invalid. Please select from one of these: SHOW, DELETE, ADD”.

3. The user must input the CMD argument in all caps. BONUS: (optional – no extra points) automatically convert the user’s CMD to uppercase.

4. If CMD is SHOW, then display all the records like this, without the quotes:

“Record 1: ID=nnn NAME=nnn AGE=nnn GPA=nnn”

Where nnn is the data from the CSV file. The record number increases for each record displayed. All the records are displayed. Use the %s, %d, and %f correctly so that the output is displayed in columns (all the ID fields are under each other, all the NAME fields are under each other, etc.). Each record in displayed on a new line. After the records are displayed the program terminates.

5. If CMD is DELETE, then there must be an OPT1 argument.

a. If this is missing, then the program terminates with the error message: “Name of record to delete is missing”.

b. If there are more arguments than OPT1, then they are ignored. This is called graceful execution. We assume the first argument is the correct OPT1 and ignore all the other arguments.

c. Delete the first record that matches ID==OPT1. The database.csv file is updated, and the program terminates. You will need to use a temporary file: database.tmp to copy the records you do not want to delete. Then use the system() command to delete the old database.csv file and rename the database.tmp file into the new database.csv file. If no record matched the search condition then display the following message and terminate: “Sorry, that user was not found. Nothing was deleted.”

6. If CMD is ADD, then there must be OPT1, OPT2, OPT3, and OPT4 arguments.

a. If less that four OPT arguments are present, terminate the program will the following error message: “Missing ID, Name, AGE, and GPA arguments”.

b. If there are more arguments, then implement graceful execution.

c. It does not matter whether another record with the same name or ID already exists. Simply append (using fopen(filename,”at”)) the new record to the end of the database.csv file.

IMPORTANT

You must use mimi.cs.mcgill.ca to create the solutions to this assignment. You cannot use your Mac command-line, Windows command-line, nor a Linux distro installed locally on your laptop. You can ssh or putty from your laptop to mimi, or you can go to the third floor of Trottier and use any of those labs, to complete this assignment.

WHAT TO HAND IN

• The database.c file

• The database.csv file

• Do not hand in the executable

• Zip all these files so that myCourses will receive them correctly.

• Make sure to add comments to your C program.

• Add your name and student ID number as a comment.

HOW IT WILL BE GRADED

THE TESTING SCRIPT

POINTS AWARDED

The assignment is worth a total of 20 points. o Question

• 2 points – correctly formatted CSV file

• 2 points – proper command line parameter testing

• 3 points – basic SHOW command works

• 4 points – basic DELETE command works

• 3 points – basic ADD command works

• 2 points – Proper use of system() for rm (delete) and cp (rename) for DELETE

• 1 point – Proper use of fopen() with append (“at”) for ADD

• 1 point – Proper use of graceful execution (two times) for DELETE &amp; ADD

• 2 points – Pretty output with SHOW

GRADING RULES

• A program must run in order to get a grade (even if it does not run well). If it does not run (does not compile) it will receive a zero. (Make sure to run your programs from mimi.cs.mcgill.ca).

• All questions are graded proportionally. This means that if 40% of the question is correct, you will receive 40% of the grade.
