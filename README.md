# Predictive_Modeling
Predict Missing Grade
Introduction

The CBSE Class 12 examination, is taken by Indian high school students at the end of K-12 school education. The scores or grades in this examination form the basis of their entry to the College or University system, for an undergraduate program. At the K-12 level, students appear for examination in five subjects. These five subjects generally include one language; three elective subjects oriented towards Science, Commerce or Humanities; and any elective of their choice as a fifth subject.


image

The Challenge

This challenge is based on real school data of the CBSE Class 12 examination conducted in the year 2013. You are given the grades obtained by students with specific but popular combinations of subjects (and all these students had opted for Mathematics). Their grades in four subjects are known to you. However their grade in Mathematics (i.e, the fifth subject) is hidden.

The records provided to you are the grades obtained by students who had opted for the following combinations of subjects or courses and obtained a passing grade in each subject. The individual subjects in the data are:
English, Physics, Chemistry, Mathematics, Computer Science, Biology, Physical Education, Economics, Accountancy and Business Studies.

The most dominant subject combinations, account for approximately 99% of the data are:

English, Physics, Chemistry, Mathematics, Computer Science    
English, Physics, Chemistry, Mathematics, Physical Education    
English, Physics, Chemistry, Mathematics, Economics    
English, Physics, Chemistry, Mathematics, Biology  
English, Economics, Accountancy, Mathematics, Business Studies    
The grades of students in four subjects (other than Mathematics) are provided to you. Can you predict what grade they had obtained in Mathematics?

To help you build a prediction engine, we will provide you with a training file, containing the grade points obtained by students with the above subject combinations, in all five subjects.

Notes about the Grading System

The student is first assessed on a scale of 100. (S)He needs a score of at least 33% to pass in the subject. Among those who pass:

Grade 1 is assigned to the top one-eighth of students who pass the course.  
Grade 2 is assigned to the next one-eighth of students who pass the course.  
.....
Grade 8 is assigned to the last one-eighth of students who pass the course.  
If more than 1 student share the same score and lie in the margin, they share the higher grade.

Input Format

The first line will be an integer N. N lines follow each line being a valid JSON object. The following fields of raw data are given in json.

SerialNumber (Numeric): The identifier of the student record. This is provided just for identification purposes and does not have any direct use.  
English (numeric) : The grade (between 1 and 8) obtained in English. This will always be present.  
Three more numeric fields from among: Physics, Chemistry, ComputerScience, Hindi, Biology, PhysicalEducation, Economics, Accountancy, BusinessStudies.  
The input for each record has the grade for all subjects opted by a student, other than Mathematics which you have to predict as the answer.

Constraints

1 <= N <= 105
The SerialNumber field will contain a unique numeric identifier such that 1 <= SerialNumber <= 5 * 105.

All other fields in the JSON fragment will represent the grades obtained in four subjects and will be populated by numeric values between 1 and 8, both inclusive.
