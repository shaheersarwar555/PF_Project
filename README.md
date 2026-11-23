# Quiz Master

A console-based multiple-choice quiz application written in **C** for the Programming Fundamentals Lab project.

## Overview

Quiz Master lets a user choose a subject and difficulty level, answer ten multiple-choice questions, view their score and percentage, and retry the quiz.

## Features

- Five subjects: English, IQ, Mathematics, General Knowledge, and Computer.
- Three difficulty levels: Easy, Medium, and Hard.
- Immediate correct/incorrect feedback.
- Score, percentage, and performance summary.
- Option to attempt another quiz.
- Saves quiz results to `QuizResults.txt`.

## Team Contributions

**Hamza Tahir**
- Developed the Mathematics, General Knowledge, and Computer sections.
- Developed the result and getValidNumber functions.
- Helped with logical proofreading and reviewing question-answer consistency.

**Shaheer Sarwar**
- Developed the English and IQ sections.
- Worked on the initial terminal text styling/bold formatting and related presentation.
- Implemented file handling for saving quiz results.

Both team members contributed to the overall project and its integration.

## How to Compile and Run

You need a C compiler such as GCC.

```bash
gcc QuizMaster.c -o QuizMaster
./QuizMaster
```

On Windows using MinGW GCC:

```bash
gcc QuizMaster.c -o QuizMaster.exe
QuizMaster.exe
```

The program creates or appends to `QuizResults.txt` in the working directory when a valid quiz result is saved.

## AI Detector Report

The AI detector screenshot and its assessment are included separately here:

[Open the AI Detector Report (PDF)](https://github.com/H-aroonTahir/Quiz-Master/blob/main/AI_Detector_Report.pdf)

The included detector result is an estimate for the text submitted to the detector. It is not definitive proof of code authorship or a measurement of the percentage of AI-generated code. AI assistance during this project was occasional and focused on debugging, logical review, and understanding specific programming issues, as described by the team.

## Project Information

- **Course:** Programming Fundamentals Lab
- **Section:** BCS-1B
- **Students:** Hamza Tahir and Shaheer Sarwar
- **Date:** 22 November 2026
- **Language:** C

## Test Scores

The following test cases were performed to check the quiz functionality, score calculation, percentage calculation, and performance feedback.

### Test Case 1: Excellent Performance

**Input:** 10 correct answers

**Output:**
```text
========== QUIZ RESULT ==========

Total Questions: 10
Correct Answers: 10
Wrong Answers: 0
Your Score: 10/10
Percentage: 100.00%
Performance: Excellent!
=================================
```

### Test Case 2: Good Performance

**Input:** 7 correct answers and 3 wrong answers

**Output:**
```text
========== QUIZ RESULT ==========

Total Questions: 10
Correct Answers: 7
Wrong Answers: 3
Your Score: 7/10
Percentage: 70.00%
Performance: Good!
=================================
```

### Test Case 3: Average Performance

**Input:** 5 correct answers and 5 wrong answers

**Output:**
```text
========== QUIZ RESULT ==========

Total Questions: 10
Correct Answers: 5
Wrong Answers: 5
Your Score: 5/10
Percentage: 50.00%
Performance: Average!
=================================
```

### Test Case 4: Needs Improvement

**Input:** 2 correct answers and 8 wrong answers

**Output:**
```text
========== QUIZ RESULT ==========

Total Questions: 10
Correct Answers: 2
Wrong Answers: 8
Your Score: 2/10
Percentage: 20.00%
Performance: Needs Improvement!
=================================
```

### Test Case 5: Invalid Input Handling

**Input:** A letter, a number outside the valid range, or an invalid menu choice.

**Expected Output:**
```text
Invalid input! Please enter a number between 1 and 4:
```

The program continues asking for input until a valid number is entered.
