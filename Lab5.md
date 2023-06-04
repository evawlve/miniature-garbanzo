Question:
=========

![Image](question.PNG)

TA/Staff Response:
==================

Answer: I see that you're having issues with the compiling of your JUnit class. Assuming that the lib folder is in the same directory as your grade.sh file, 
what is the command within the bash file that is being used to compile? I noticed that your operating system is Windows based and a common bug found with the 
Windows systems is the compiling of the JUnit class. 

Student Reply:
==============

When attempting to run the bash file, I this error in the terminal. Included in the screenshot is the diretories being used and the contents of the bash.sh file being used to grade the ListExamples.java files.

![Image](studentissue.PNG)

TA/Staff Response:
==================
Answer: Like I mentioned earlier, I can see that the issue could be caused by how you're compiling the JUnit. You can try changing line 34 of your grade.sh bash file, to being:
java -cp ".;lib/junit-4.13.2.jar;lib/hamcrest-core-1.3.jar" org.junit.runner.JUnitCore TestListExamples > results.txt
The difference being the semicolon before "lib" instead of the colon. 

Student Reply:
==============

It works! I changed the colon to the semi as you advised me to do so, and now the grade.sh file is correctly grading the filee, thank you so much for the help!!

![Image](fix.PNG)
