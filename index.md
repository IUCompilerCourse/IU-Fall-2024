## Course Webpage for Compilers (P423, P523, E313, and E513)

Indiana University, Fall 2024


High-level programming languages like Racket and Python make it easier
to program compared to low-level languages such as x86 assembly
code. But how do high-level languages work? There's a big gap between
them and machine instructions for modern computers. In this class you
learn how to translate Racket or Python programs (your choice!) all
the way to x86 assembly language.

Traditionally, compiler courses teach one phase of the compiler at a
time, such as parsing, semantic analysis, and register allocation. The
problem with that approach is it is difficult to understand how the
whole compiler fits together and why each phase is designed the way it
is. Instead, each week we implement a progressively larger subset of
the input language. The very first subset is a tiny language of
integer arithmetic, and by the time we are done the language includes
first-class functions.

**Prerequisites:** Fluency in Racket or Python is highly recommended
as students will do a lot of programming in one of those
languages. Prior knowledge of an assembly language helps, but is not
required.

**Textbook: Essentials of Compilation: An Incremental Approach in Racket/Python** 

* The Racket version of the textbook for the course is available at
  the IU bookstore and from many book sellers, links to those
  [here](https://mitpress.mit.edu/9780262047760/essentials-of-compilation/).
  The PDF is also available for free
  [here](https://www.dropbox.com/s/ktdw8j0adcc44r0/book.pdf?dl=1).
  
* The Python version of the textbook for the course is available
  at the IU bookstore and from many book sellers, links to those
  [here](https://mitpress.mit.edu/9780262048248/essentials-of-compilation/).
  The PDF is also available for free
  [here](https://www.dropbox.com/s/mfxtojk4yif3toj/python-book.pdf?dl=1).

If you have suggestions for improvement, please either send an email
to Jeremy or, even better, make edits to a branch of the book and
perform a pull request. The book is at the following location on
github:

    https://github.com/IUCompilerCourse/Essentials-of-Compilation


**Lecture:** Tuesdays and Thursdays 3:00-4:15pm, Informatics Building
  (Myles Brand Hall), Room I 107.


**Office hours**

* Jeremy Siek (jsiek): TBD in Luddy 3014 (or nearby).
* Darshal Shetty (dcshetty): TBD.


**Topics:**

* Instruction Selection

* Register Allocation

* Static type checking

* Conditional control flow

* Mutable data

* Garbage collection

* Procedures and calling conventions

* First-class functions and closure conversion

* Dynamic typing

* Generics

**Grading:**

Course grades are based on the following items. For the weighting, see
the Canvas panel on the right-hand side of this web page.  Grading
will take into account any technology problems that arrise, i.e., you
won't fail the class because your internet went out.

* Assignments (40%)
* Midterm Exam (25%)
* Final Exam (35%)

**Assignments:**

Organize into teams of 2-4 students. Assignments will be due bi-weekly
on Mondays at 11:59pm. Teams that include one or more graduate
students are required to complete one challenge exercise per
assignment.

Assignment descriptions are posted on Canvas.  Turn in your
assignments by submitting your code to the autograder.  There is a
Racket and Python version of each assignment.  Submit your `compiler`
file, either `compiler.rkt` or `compiler.py` depending on the language
you are using.

Assignments will be graded based on how many test cases they succeed
on. Partial credit will be given for each "pass" of the compiler.
Some of the tests are in the public support code (see Resources
below). The testing will be done on a linux (ubuntu) machine. The
testing will include both new tests and all of the tests from prior
assignments.

You may request feedback on your assignments prior to the due date.
Just submit your work to the autograder and send us email.

Students are responsible for understanding the entire assignment and
all of the code that their team produces. The midterm and final exam
are designed to test a student's understanding of the assignments.

Students are free to discuss and get help on the assignments from
anyone or anywhere. When posting questions on Slack, it is OK to post
your code.

In contrast, for quizzes and exams, students are asked to work
alone. The quizzes and exams are closed book.


**Late assignment policy:** Assignments may be turned in up to one
week late with a penalty of 10%.

**Slack Chat/Messaging:**
  [Workspace](https:://compilersfall2024.slack.com) 
    ([signup](https://join.slack.com/t/slack-b668831/shared_invite/zt-2p75mnh2b-0iLe8d8Bj1UuEj0ivh_nTg)
  using your iu email address).

**Schedule**

Day     | Lecture Topic              | Assignment Due
Aug. 27 | [Introduction](https://docs.google.com/presentation/d/13jmEAwqD7naNAj0c2IsF0tDhgMyQH-tBW9sZeRgzBt8/edit?usp=sharing)               |
Aug. 29 | [From Lvar to x86](https://docs.google.com/presentation/d/1KUlWTAvdcKtZNOST9ITpmiOe34lD2DFsycH5oT2oMuU/edit?usp=sharing) |
Sep. 3 | [Uniquify, Remove Complex Operands, Explicate Control](https://docs.google.com/presentation/d/1KIFtThQVM-u9DVttCT4q_68CVCTlIq_WCUwBOhdaB3o/edit?usp=sharing), [video](https://iu.mediaspace.kaltura.com/media/t/1_l0szlnzg) |
Sep. 5 | [Explicate Control through Prelude & Conclusion](https://docs.google.com/presentation/d/1KUlWTAvdcKtZNOST9ITpmiOe34lD2DFsycH5oT2oMuU/edit?usp=sharing), [video](https://iu.mediaspace.kaltura.com/media/t/1_t431x6fs) |
Sep. 10  | [Register Allocation, Introduction and Liveness](https://docs.google.com/presentation/d/1jL4M6G6DDnfqOPsCab9_6k7PcV_wRBd4p9Xn2LzobOE/edit?usp=sharing) | Integers and Variables, submit in [Racket](https://autograder.luddy.indiana.edu/web/project/1280) or [Python](https://autograder.luddy.indiana.edu/web/project/1283)
Sep. 12  | Code Review: Integers and Variables
Sep. 17 | [Register Allocation: graph coloring](https://docs.google.com/presentation/d/1qPKUGZnqh6ggfP5_emHVJhSTyPRI0iD02jRTdB9mbwo/edit?usp=sharing) | Integers and Variables, late deadline
Oct. 24 | **Midterm Exam** in class
Dec. 19 | **Final Exam** 3-5pm

**Resources:**

* Practice exams:
  - Midterm from 2022: [Python](./2022-python-midterm.pdf), [Python with solutions](./2022-python-midterm-soln.pdf), [Racket](./2022-racket-midterm.pdf), [Racket with solutions](./2022-racket-midterm-soln.pdf)
  - Final from 2022: [Python](./2022-python-final.pdf), [Python with solutions](./2022-python-final-soln.pdf), [Racket](./2022-racket-final.pdf), [Racket with solutions](./2022-racket-final-soln.pdf)
  - Final from 2021: [Python](./2021-python-final.pdf), [Python with solutions](./2021-python-final-soln.pdf), [Racket](./2021-racket-final.pdf), [Racket with solutions](./2021-racket-final-soln.pdf)
  
* Lecture videos recorded from the [2020 course](https://iucompilercourse.github.io/IU-P423-P523-E313-E513-Fall-2020/).
* Github repository for the support code and test suites
    - for [Racket](https://github.com/IUCompilerCourse/public-student-support-code) 
	- for [Python](https://github.com/IUCompilerCourse/python-student-support-code)
* [Racket Download](https://download.racket-lang.org/)
* [Racket Documentation](https://docs.racket-lang.org/)
* [Python Download](https://www.python.org/downloads/)
* [Python Documentation](https://docs.python.org/)
* [Python ast module declarations](https://github.com/python/typeshed/blob/master/stdlib/_ast.pyi)
* [Notes on x86-64 programming](http://web.cecs.pdx.edu/~apt/cs491/x86-64.pdf)
* [x86-64 Machine-Level Programming](https://www.cs.cmu.edu/~fp/courses/15411-f13/misc/asm64-handout.pdf)
* [Intel x86 Manual](http://www.intel.com/content/dam/www/public/us/en/documents/manuals/64-ia-32-architectures-software-developer-manual-325462.pdf?_ga=1.200286509.2020252148.1452195021)
* [System V Application Binary Interface](https://software.intel.com/sites/default/files/article/402129/mpx-linux64-abi.pdf)
* [Uniprocessor Garbage Collection Techniques](https://iu.instructure.com/courses/1735985/files/82131907/download?wrap=1) by Wilson. 
* [Fast and Effective Procedure Inlining](https://www.cs.indiana.edu/~dyb/pubs/inlining.pdf) by Waddell and Dybvig.


**Bias-Based Incident Reporting.**

Bias-based incident reports can be made by students, faculty and
staff. Any act of discrimination or harassment based on race,
ethnicity, religious affiliation, gender, gender identity, sexual
orientation or disability can be reported through any of the options:

1) email biasincident@indiana.edu or incident@indiana.edu;

2) call the Dean of Students Office at (812) 855-8188 or

3) use the IU mobile App (m.iu.edu). Reports can be made anonymously.

**Dean on Call.**

The Dean of Students office provides support for students dealing with
serious or emergency situations after 5 p.m. in which an immediate
response is needed and which cannot wait until the next business
day. Faculty or staff who are concerned about a student’s welfare
should feel free to call the Dean on Call at (812) 856-7774. This
number is not to be given to students or families but is for internal
campus use only. If someone is in immediate danger or experiencing an
emergency, call 911.

**Boost.**

Indiana University has developed an award-winning smartphone app to
help students stay on top of their schoolwork in Canvas. The app is
called “Boost,” it is available for free to all IU students, and it
integrates with Canvas to provide reminders about deadlines and other
helpful notifications. For more information, see
https://kb.iu.edu/d/atud.

**Counseling and Psychological Services.**

CAPS has expanded their services. For information about the variety of
services offered to students by CAPS visit:
http://healthcenter.indiana.edu/counseling/index.shtml.


**Disability Services for Students (DSS).**

The process to establish accommodations for a student with a
disability is a responsibility shared by the student and the DSS
Office. Only DSS approved accommodations should be utilized in the
classroom. After the student has met with DSS, it is the student’s
responsibility to share their accommodations with the faculty
member. For information about support services or accommodations
available to students with disabilities and for the procedures to be
followed by students and instructors, please visit:
https://studentaffairs.indiana.edu/disability-services-students/.

**Reporting Conduct and Student Wellness Concerns.**

All members of the IU community including faculty and staff may report
student conduct and wellness concerns to the Division of Student
Affairs using an online form located at
https://studentaffairs.indiana.edu/dean-students/student-concern/index.shtml.

**Students needing additional financial or other assistance.**

The Student Advocates Office (SAO) can help students work through
personal and academic problems as well as financial difficulties and
concerns. SAO also assists students working through grade appeals and
withdrawals from all classes. SAO also has emergency funds for IU
students experiencing emergency financial crisis
https://studentaffairs.indiana.edu/student- advocates/.

**Disruptive Students.**

If instructors are confronted by threatening behaviors from students
their first obligation is to insure the immediate safety of the
classroom. When in doubt, call IU Police at 9-911 from any campus
phone or call (812) 855-4111 from off-campus for immediate or
emergency situations. You may also contact the Dean of Students Office
at (812) 855-8188. For additional guidance in dealing with difficult
student situations:
https://ufc.iu.edu/doc/policies/disruptive-students.pdf.

**Academic Misconduct.**

If you suspect that a student has cheated, plagiarized or otherwise committed academic misconduct, refer to the Code of Student Rights, Responsibilities and Conduct:
http://studentcode.iu.edu/.

**Sexual Misconduct.**

As your instructor, one of my responsibilities is to create a positive
learning environment for all students. Title IX and IU’s Sexual
Misconduct Policy prohibit sexual misconduct in any form, including
sexual harassment, sexual assault, stalking, and dating and domestic
violence. If you have experienced sexual misconduct, or know someone
who has, the University can help.

If you are seeking help and would like to speak to someone
confidentially, you can make an appointment with:

* The Sexual Assault Crisis Services (SACS) at (812) 855-8900
  (counseling services)

* Confidential Victim Advocates (CVA) at (812) 856-2469 (advocacy and
  advice services)

* IU Health Center at (812) 855-4011 (health and medical services)

It is also important that you know that Title IX and University policy
require me to share any information brought to my attention about
potential sexual misconduct, with the campus Deputy Title IX
Coordinator or IU’s Title IX Coordinator. In that event, those
individuals will work to ensure that appropriate measures are taken
and resources are made available. Protecting student privacy is of
utmost concern, and information will only be shared with those that
need to know to ensure the University can respond and assist.  I
encourage you to visit
stopsexualviolence.iu.edu to learn more.
