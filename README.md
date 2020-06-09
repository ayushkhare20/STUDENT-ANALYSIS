# STUDENT-ANALYSIS
DESCRIPTION

A university wants to categorize the marks scored by the students of each batch in the quizzes conducted.
Datasets:

studentlist.csv is a csv file (attached) which includes the student details like enrollmentnumber, admissionno. Batchwiselist is a folder(attached) which has multiple csv files.
Each file contains the student details belonging to a batch. For example, 1.csv contains the student details belonging to batch1 and 2.csv contains the student details belonging
to batch2 and so on.quiz is a folder(attached) which has multiple csv files. Each file represents a quiz conducted by the university and contains all the important details. The column 'Grade/10.00' contains the marks obtained in that quiz out of maximum marks of 10. For example quiz1.csv contains the student details and the marks obtained by them in the first quiz.

Now you need to perform the following steps on this data:

1.	Read the file studentlist.csv

2.	Read the files present in the folders batchwiselist, quiz

3.	Manipulate the data and create a Statistics dataframe in such a way that it allocates marks to the students of each batch for the quizzes. Statistics dataframe for each batch
should include the following column names with the respective statistics value. The column names infer the meaning of each column.

["noofpresent", "lessthan50", "between50and60", "between60and70", "between70and80", "greaterthan80"]

•	Rows of Statistics dataframe represents the quiz. Such as, the first row under the column “between50and60” represents the number of students whose percentage is in between
50 and 60 in the first quiz.

•	The second row under the column “between50and60” represents the number of students whose percentage is in between 50 and 60 in the second quiz.

•	The first row under the column "noofpresent" represents the number of students who attempted the first quiz from that batch.

•	The second row under the column "noofpresent" represents the number of students who attempted the second quiz from that batch.

Input Format

You must read a file named testcaseStudent.txt (attached) which has the following lines: The first line contains the number of testcase pairs.

Followed by a set of Batch file and Percentage range pairs.

Output Format

For each testcase pair n, create an output file outputn.txt where n represents the test case pair number.

This file should contain the number of students who got marks in the requested percentage range from that batch.

outputn.txt should consist of the values in a separate line for each quiz.
 



Sample Test Cases Sample Input

testcaseStudent.txt contains the following data:

2
4.	csv greaterthan80 3.csv lessthan50 Sample Output


output1.txt contains the following data:

12
45
output2.txt contains the following data:

10
15


Explanation
As there are two quiz files in the quiz folder, output file should consist of two values, each value representing a quiz.

In the batch 4.csv, there are 12 students who scored greater than 80 in the first quiz and 45 students in second quiz

In the batch 3.csv, there are 10 students who scored less than 50 in the first quiz and 15 students in second quiz.



Note : This assignment will require use of os.listdir(), to list all the files available in any particular directory/folder.
