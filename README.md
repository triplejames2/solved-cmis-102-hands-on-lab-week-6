Download Link: https://assignmentchef.com/product/solved-cmis-102-hands-on-lab-week-6
<br>
<strong>Overview </strong>

This hands-on lab allows you to follow and experiment with the critical steps of developing a program including the program description, analysis, test plan, design and implementation with C code. The example provided uses sequential, repetition statements and nested repetition statements.

<strong> Program Description </strong>

This program will calculate the average of 3 exams for 5 students. The program will ask the user to enter 5 student names. For each of the students, the program will ask for 3 exam scores. The average exam score for each student will be calculated and printed.

<strong>Analysis</strong>

I will use sequential and repetition programming statements. I will define one String to store the student name: StudentName. I will define three Float numbers: Examvalue, Sum, Avg to store exam values the sum of the exams and the average of the exams. The sum will be calculated by this formula:

Sum = Sum + Examvalue For example, if the first value entered was 80.0 and second was 90.0 and the third exam was 100.0: sum = sum + Examvalue = 0.0 + 80.0 sum = 80.0 + 90.0 = 170.0 sum = 170.0 + 100.0 = 270.0 Avg is then calculated as: Avg = sum/3.0 For example 270.0/3.0 = 90.0 A nested repetition loop can be used to loop through each of the 5 students and each of the 3 exams: For (students=0; students &lt;5; students++) For (exams=0;exams&lt;3;exams++) End For End For Sum values will need to be reset for each student to ensure only one student data is used for calculations each time.

<strong>Test Plan </strong>

To verify this program is working properly the input values could be used for testing: Test Case Input Expected Output 1 Studentname=Chris Examvalue1=80.0 Examvalue2=90.0 Examvalue3=100.0 Average for Chris is 90.0 Average for John is 80.0 Average for Sally is 100.0 2 Studentname=John Examvalue1=70.0 Examvalue2=90.0 Examvalue3=80.0 Studentname=Sally Examvalue1=100.0 Examvalue2=100.0 Examvalue3=100.0 Studentname=Pat Examvalue1=50.0 Eexamvalue2=70.0 Examvalue3=60.0 Studentname=Sam Examvalue1=90.0 Examvalue2=95.0 Examvalue3=100.0 Average for Pat is 60.0 Average for Sam is 95.0

<strong>Pseudocode </strong>

// This program will calculate the average of 3 exams for 5 students // Declare variables Declare StudentName as String Declare ExamValue, Sum, Avg as Float // Loop through 5 Students For (students=0; students &lt;5 ; students++) // reset Sum to 0 Set Sum =0.0 Print “Enter Student Name” Input StudentName // Nested Loop for Exams For (exams=0; exams &lt; 3; exams++) Print “Enter exam grade: 
” Input ExamValue Set Sum = Sum + ExamValue End For Set Avg = Sum/3.0 Print “Average for “ + StudentName + “ is “ + Avg End For 3

<strong>C Code </strong>

The following is the C Code that will compile in execute in the online compilers. // C code // This program will calculate the average of 3 exams for 5 students. // Developer: Faculty CMIS102 // Date: Jan 31, XXXX #include int main () { /* variable definition: */ char StudentName[100]; float ExamValue, Sum, Avg; int students,exams; // Loop through 5 Students for (students=0; students &lt;5 ; students++) { // reset Sum to 0 Sum =0.0; printf(“Enter Student Name 
”); scanf(“%s”, StudentName); // Nested Loop for Exams for (exams=0; exams &lt; 3; exams++) { printf (“Enter exam grade: 
”); scanf(“%f”, &amp;ExamValue); Sum += ExamValue; } Avg = Sum/3.0; printf( “Average for %s is %f
”,StudentName,Avg); } return 0; } 4 Setting up the code and the input parameters in ideone.com: Note the Student and ExamValues for this run were: John: 90.0 80.0 100.0 Jim: 80.0 70.0 90.0 Joe: 70.0 100.0 100.0 Sally: 100.0 95.0 91.0 Sam: 30.0 54.0 68.0 You can change these values to any valid integer values to match your test cases.

<strong>Results from running the programming at ideone.com</strong>

<strong> Learning Exercises for you to complete</strong>

1. Demonstrate you successfully followed the steps in this lab by preparing screen captures of you running the lab as specified in the Instructions above.

2. Modify the code to be able to input an undetermined number of students. You will still only have 3 exams for each student. Support your experimentation with screen captures of executing the new code.

3. Prepare a new test table with at least 3 distinct test cases listing input and expected output for the code you created after step 1.

4. What is the line of code doing? char StudentName[100]; (Hint: We haven’t covered arrays, but a String can be thought of as an array of characters) ? 6

5. What would happen if you moved the Set Sum = 0.0 from inside the for loop to right after the declaration. For example: // Declare variables Declare StudentName as String Declare ExamValue, Sum, Avg as Float // Initialize Sum Set Sum = 0.0; Support your experimentation with screen captures of executing the new code.