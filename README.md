# Course 3: Functional Programming in R
This repository will house all the materials for the third course in the data science specialization using R, developed for the UO COE.

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

# Syllabus
## EDLD XXX: Functional Programming in R (CRN: XXXXX; 3 credit hours)
* **Term:**
* **Time:** 
* **Classroom:** 
* **Instructor:** Daniel Anderson, PhD
	+ *email:* (preferred contact method) [daniela@uoregon.edu](mailto:daniela@uoregon.edu)
	+ *phone:* 541-346-3317
	+ *office:* 175 Lokey
	+ *office hours*: 

# Course Overview
This is the third course in a sequence of courses that will eventually lead to 
a *data science in educational research* specialization. This course will be taught
through [R](https://cran.r-project.org), a free and open-source statistical
computing environment. This course, in particular, will rely heavily on building
on the first two courses using [RStudio]. Here the focus is on becoming
a better programmer with R and improving workflows in statistical computing with R.
Students will continue to work with the [tidyverse](https://www.tidyverse.org) 
suite of packages mostly using the {purrr} package, while
also comparing and contrasting with base R techniques like `for` loops and the `apply`
set of functions. Lastly, the course concludes with a two week dive into [shiny](https://shiny.rstudio.com/)
culminating the experience of writing functions and functional programming with a
final project of the student's choosing.

## Student Learning objectives
By the end of this course, students should be able to:
* Assess the differences in R's data structures (vectors, data frames, lists) and when each is most appropriate
* Work with lists and list columns using `purrr::nest` and `purrr:unnest`
* Fit multiple models using the {broom} package with the {purrr} package
* Convert repetitive tasks into functions and test them for effectiveness
* Decipher what makes a good function and good assertions on parameters
* Write effective and clear functions to continue with the mantra of "Don't Repeat Yourself"
* Explore `purrr::map` and its variants
* Understand how `purrr::map` differs from base functions, and why its preferable
* Convert previous code written in prior courses to be more in the functional programming spirit
* Build their first shiny app related to their work/research

# Course Reading List And Other Resources
All course readings are freely available online or will be provided by the
instructor. 

## Books (required)
* Bryan, J. (2018). *[Happy git and GitHub for the useR](http://happygitwithr.com)*. [@datalorax, not sure if this will be needed for this course?]
* Ismay, C. and Kim, A. Y. (2018). *[ModernDive: An introduction to statistical and data sciences via R](http://www.moderndive.com)*.
* Wickham, H. and Grolemund, G. (2017). *[R for data science](http://r4ds.had.co.nz)*. Sebastopol, CA: O'Reilly. 
	+ Freely available online in the link above. A full-color paper copy is also [available from Amazon](http://amzn.to/2aHLAQ1) for (currently) \$18.17.

## Resources
### [DataCamp](https://www.datacamp.com)
We have a class subscription to [DataCamp](https://www.datacamp.com). This means all the courses
they offer (which is a lot) are available to you. I encourage you to explore the website and
play around. There are **far more** topics covered by DataCamp than we will cover in this
course or this five-course specialization.

In addition to having DataCamp as a resource for your own exploration of topics not covered
by this class, we will use DataCamp content to supplement lectures, and as a place for you
to practice the skills you learn in class.

Our DataCamp website is located [here](https://www.datacamp.com/enterprise/introduction-to-data-science-with-r). 
I suggest bookmarking the page as we will use it throughout the term.


# Weekly Schedule (Topics, Assignments, and Readings)
| **Week** | **Theme**                                         | **Topics**                                                | **Assignment Assigned**                  | **Assignment Due**                       | **Reading**                                                         |
|----------|---------------------------------------------------|-----------------------------------------------------------|------------------------------------------|------------------------------------------|---------------------------------------------------------------------|
| 1a       | Data Types 1                                      | vectors, matrices, lists, data frames                     | DC: Introduction to R                    | -                                        | http://adv-r.had.co.nz/Data-structures.html                         |
| 1b       | Data Types 2                                      | factors                                                   | DC: Intermediate R 1-2                   | DC: Introduction to R                    | http://adv-r.had.co.nz/Data-structures.html                         |
| 2a       | Introduction to iteration 1                       | for loops and the apply functions                         | DC: Intermediate R 3-5                   | DC: Intermediate R 1-2                   | https://www.datacamp.com/community/tutorials/tutorial-on-loops-in-r |
| 2b       | Introduction to iteration 2                       | purrr: map, map_df, map_dbl, map_chr, map_lgl, map_int    | CW Challenges                            | DC: Intermediate R 3-5                   | https://github.com/jenniferthompson/RLadiesIntroToPurrr             |
| 3a       | Introduction to iteration 3                       | purrr: map2, and friends                                  | DC: purrr course (To be launched)        | CW Challenges                            | https://github.com/jenniferthompson/RLadiesIntroToPurrr             |
| 3b       | Introduction to iteration 4                       | tidyr::crossing(), purrr::safely()                        | DC: purrr course (To be launched)        | DC: purrr course (To be launched)        | https://colinfay.me/purrr-adverb-tidyverse/                         |
| 4a       | Nesting and unnesting data                        | purrr::nest and purrr::unnest                             | DC: second purrr course (To be launched) | DC: purrr course (To be launched)        | http://r4ds.had.co.nz/many-models.html                              |
| 4b       | Fitting multiple models                           | purrr with broom                                          | DC: ML in the Tidyverse 1                | DC: second purrr course (To be launched) | http://r4ds.had.co.nz/many-models.html                              |
| 5a       | Introduction to lists (and data frames as lists)  | Nesting of URLs, html code with rvest with purrr          | DC: ML in the Tidyverse 2                | DC: ML in the Tidyverse 1                | http://r4ds.had.co.nz/lists.html                                    |
| 5b       | fs package, batch load data, and map_df           | Loading in data, understanding directory architecture     | purrr project                            | DC: ML in the Tidyverse 2                | https://www.tidyverse.org/articles/2018/01/fs-1.0.0/                |
| 6a       | Writing functions 1                               | The basics of writing functions to reduce copying of code | DC: Hadley & Charlotte 1-2               | First checkin on purrr project           | http://r4ds.had.co.nz/functions.html                                |
| 6b       | Writing functions 2                               | Making tweaks to functions to improve readability and use | Continue on purrr project                | DC: Hadley & Charlotte 1-2               | https://swcarpentry.github.io/r-novice-inflammation/02-func-R/      |
| 7a       | Putting it all together: Functional Programming 1 | Review lapply, functions, anonymous functions             | DC: Hadley & Charlotte 3-5               | purrr project due                        | http://adv-r.had.co.nz/Functional-programming.html                  |
| 7b       | Putting it all together: Functional Programming 2 | Closures, mutable states                                  | DC: Mine shiny 1-2, Final project        | DC: Hadley & Charlotte 3-5               | http://adv-r.had.co.nz/Functional-programming.html                  |
| 8a       | Shiny 1                                           | Basics of shiny: server and ui                            | DC: Mine shiny 3-4                       | DC: Mine shiny 1-2                       | https://shiny.rstudio.com/                                          |
| 8b       | Shiny 2                                           | Reactive programming, customization                       | DC: Dean shiny 1-2                       | DC: Mine shiny 3-4                       | https://shiny.rstudio.com/                                          |
| 9a       | Shiny 3                                           | Shiny review                                              | DC: Dean shiny 3-4                       | DC: Dean shiny 1-2                       | https://shiny.rstudio.com/                                          |
| 9b       | Shiny 4                                           | Interactivity                                             | Work on final project                    | DC: Dean shiny 3-4                       | https://shiny.rstudio.com/                                          |
| 10a      | Finishing projects                                |                                                           |                                          |                                          |                                                                     |
| 10b      | Finishing projects                                |                                                           |                                          |                                          |                                                                     |

The final project will likely take one of three forms: R Markdown website, a reproducible document showing learning throughout the course, or a Shiny app.

# Assignments 
As outlined in the table above, most class meetings will include a lab. All 
labs will also count toward homework assignments, with roughly half the 
assignment completed during lab, and the other half completed out of class. 
The DataCamp platform will also be used for additional homework assignments, 
and the course will conclude with a final project. More detail about each is 
provided below.

## Homework (XXX points; XX%)
 
 <!--
### Labs (140 points)
There are 14 labs during the course, which must be submitted to the instructor
prior to the start of the following class. These labs will be scored on a "best
honest effort" basis, which generally implies zero or full credit (i.e., the
assignment was or was not fully completed). However, many of the labs require
students complete specific portions before moving on to the next sections. If
you find yourself stuck and unable to proceed, **please contact the instructor
for help rather than submitting incomplete work**. Contacting the instructor
is part of the "best honest effort", and can result in full credit for an 
assignment even if the the work is not fully complete. **If the assignment is
not complete, and the student has not contacted the instructor for help or
visited office hours, it is likely to result is a score of zero**.
-->

### DataCamp Chapters (XX points)
DataCamp is an excellent resource to  get additional instruction and/or go 
more in-depth on any of the topics covered in this class. There are also some 
topics that we will not have the time to cover in much detail, and DataCamp 
can be helpful for these topics as well. However, in addition to providing 
supplemental support, select chapters will be assigned and scored as part of 
homework, at **five points per chapter**. A total of 17 chapters will be
assigned (note that many of these chapters are very brief).

## Final Project (XXX points; XX%)

**To be finalized with Daniel**

@datalorax: Will students be expected to be using their own research data by
this point in the curriculum? How broad do you want this to be in terms of what students
can do?

The final project in this class is a group project, requiring students use a 
“real world” dataset to write, essentially, a miniature manuscript, including 
an introduction (paragraph or two), methods, results, and discussion (again, 
maybe 2-3 paragraphs). Ideally, students would work with a dataset that 
includes variables they are interested in using beyond just this class; 
however, if students do not have access to a dataset, the instructor will
provide one. **Students who do not have access to data should plan to meet with
the instructor as soon as possible so a dataset can be provided**. 
Additionally, **the dataset must be able to be shared publicly**, as the full
project will be required to be housed on GitHub and be fully reproducible. If 
making your data publicly available is a problem for you, please contact the 
instructor as soon as possible. We can work together to either find a dataset 
that will work for you, or simulate a dataset that is similar to the data 
you'd like to work with in reality (and then all your code should work for the 
real dataset, but you can share the simulated data with your classmates). 
Students are required to work in groups of 2-4 people. The final assignment is 
assigned during the first class, and **groups must be finalized by the end of 
Week 2** (at which point students who have not self-selected into groups will 
be randomly assigned).

<!--
### Outline (XX points)
A basic outline of the final project is due at the end of Week 5. The outline 
should include a description of the data to be used, a discussion of what 
preparatory work will need to be done and how the requirements of the final 
project will be met. The outline is intended to be low-stakes and is primarily 
designed to be a means for you to obtain feedback on the feasibility of the 
project and areas to consider. 

### Draft Data Preparation Script (25 points)
At the end of Week 8, you must have a draft of the data preparation complete, 
including moving the data from its raw to tidy form and a variety of 
exploratory data visualizations.

### Peer Review of Data Preparation Script (25 points)
Following the submission of the data preparation scripts, you will be assigned 
to review your peers code. The purpose of this exercise is to learn from each 
other. Programming is an immensely open-ended enterprise and there are lots of 
winding paths that all ultimately end up at the same destination. During your 
peer review, you must note (a) at least three areas of strength, (b) at least 
one thing you learned from reviewing their script, and (c) at least one and no
more than three areas for improvement. 

Making your code publicly available can feel daunting. The purpose of this 
portion of the final project is to help us all learn from each other, not to 
denigrate. **Under no circumstances will negative comments be tolerated**. Any 
comments that could be perceived as negative, and outside the scope of the 
code, will result in an immediate score of zero. Be constructive in your 
feedback. Be kind. We are all learning.

### Final Project Presentation (25 points)
Each group will present on their final project during Week 10, which is 
expected to still be in progress. These presentations are expected to be 
informal, and emphasize what learning occurred during the project.
Specifically, the presentations are to commiserate with each other about the
failures and challenges experienced along the way, while also celebrating the 
successes. Learning R is a difficult task, and we should all take solace 
knowing that others are struggling along with us. The final presentation 
should be equal parts “journey” and substantive findings/conclusions/results. 
Students are expected to present for approximately 10 minutes each (20-40 
minutes per group), although the time may change depending on the enrollment 
of the class.
 

### Final Paper (110)
The purpose of the final project is to allow students an opportunity to
demonstrate all the skills they have learned throughout the course. The final
project must (a) be a reproducible and dynamic APA manuscript produced with R
Markdown, via the [*{papaja}*](https://github.com/crsh/papaja) package and
include references to the extant literature; (b) be housed on GitHub, with
contributions from all authors obvious; (b) demonstrate
moving data from its raw “messy” format to a tidy data format through the R Markdown file, but not in the final document; (c) include at least two exploratory data visualizations, and (d) include at least summary statistics of the data in tables, although fitted models of any sort are an added bonus (not literally, there are not extra points for fitting a model). The points for the final project are broken down as follows:

* Writing (abstract, intro, methods, results, discussion, references): 30 points (25%)
* Document is fully reproducible and housed on GitHub: 25 points (21%)
* Demonstrate use of inline code: 5 points (4%)
* Demonstrate tidying messy data: 30 points (25%)
* Two data visualizations: 10 points each, 20 points total (17%)
* Production of at least one table (of summary statistics or model results): 10 points (8%)

I will investigate the commits made by different authors when evaluating the
final project. If it is obvious that one person did not utilize GitHub, and
instead added all of their contributions through a single or only a few 
commits, I will dock points from that individual. There should be numerous
commits by each author, and they should be roughly even in terms of
contribution activity (which GitHub has metrics to track, both in terms of the
number of commits as well as the number of lines modified).

-->

# Grading Components
|  **Lower percent** |**Lower point range**  | **Grade** | **Upper point range**  | **Upper percent**|
|  :------: | :------   | :-:| :-------: | ----:|
|  0.97     | (422 pts) | A+ |           |      |
|  0.93     | (405 pts) | A  | (422 pts) | 0.97 |
|  0.90     | (392 pts) | A- | (405 pts) | 0.93 |
|  0.87     | (378 pts) | B+ | (392 pts) | 0.90 |
|  0.83     | (361 pts) | B  | (378 pts) | 0.87 |
|  0.80     | (348 pts) | B- | (361 pts) | 0.83 |
|  0.77     | (335 pts) | C+ | (348 pts) | 0.80 |
|  0.73     | (318 pts) | C  | (335 pts) | 0.77 |
|  0.70     | (304 pts) | C- | (318 pts) | 0.73 |
|           |           | F  | (304 pts) | 0.70 |

# Student Engagement Inventory
Graduate: 1 credit hour = 40 hours of student engagement (3 credit hours = 120 hours of student engagement) 

| **Educational activity** | **Hours student engaged** | **Explanatory comments (if any):**                                                                               |
| :----------------------- | :-----------------------: | :--------------------------------------------------------------------------------------------------------------- |
| Course attendance        |            26.5             | 20 meetings, at 80 minutes per meeting                                                                           |
| Assigned readings        |            27             | Weekly readings are assigned, and are expected to take roughly as long to complete as the in-seat time per week. |
| Projects                 |            30             | Final project, as described above                                                                                |
| Homeworks                |            36.5           | 14 Labs, at approximately two hours per lab spent out of class (28 hours), plus 17 DataCamp chapters, at approximately 0.5 hours per chapter |
| Total hours:             |            120            |                                                                                                                  |

# Attendance and Absence Guidelines
Attendance at all class and discussion groups is expected and required, as described above.

Students must contact the instructor in case of illness or emergencies that preclude attending class sessions. Messages can be left on the instructor's voice mail or e-mail at any time of the day or night, prior to class. If no prior arrangements have been made before class time, the absence will be unexcused. Excused absences will involve make-up assignments, with make-up assignment procedures to be discussed in class on the first day. 

If you are unable to complete an assignment due to a personal and/or family emergency, you should contact your instructor or discussion leader as soon as possible. On a case-by-case basis, the instructor will determine whether the emergency qualifies as an excused absence. 

# Expected Classroom Behavior
Students are expected to participate in classroom activities. If use of digital devices or engagement in other non-class activities during class for purposes not regarding classroom activities is critically necessary, the student should engage in these activities while on break, or check with the instructor to arrange for a 10-minute break for unusual circumstances, but only if critically necessary. 

# Course Policies 
## Diversity, Equity and Inclusion
It is the policy of the University of Oregon to support and value equity and diversity and to provide inclusive learning environments for all students.  To do so requires that we: 

* respect the dignity and essential worth of all individuals. 
* promote a culture of respect throughout the University community. 
* respect the privacy, property, and freedom of others. 
* reject bigotry, discrimination, violence, or intimidation of any kind. 
* practice personal and academic integrity and expect it from others. 
* promote the diversity of opinions, ideas and backgrounds which is the lifeblood of the university.

In this course, class discussions, projects/activities and assignments will challenge students to think critically about and be sensitive to the influence, and intersections, of race, ethnicity, nationality, documentation status, language, religion, gender, socioeconomic background, physical and cognitive ability, sexual orientation, and other cultural identities and experiences. Students will be encouraged to develop or expand their respect and understanding of such differences.

Maintaining an inclusive classroom environment where all students feel able to talk about their cultural identities and experiences, ideas, beliefs, and values will not only be my responsibility, but the responsibility of each class member as well. Behavior that disregards or diminishes another student will not be permitted for any reason. This means that no racist, ableist, transphobic, xenophobic, chauvinistic or otherwise derogatory comments will be allowed. It also means that students must pay attention and listen respectfully to each other’s comments.

## Documented Disability
Appropriate accommodations will be provided for students with documented disabilities. If you have a documented disability and require accommodation, arrange to meet with the course instructor within the first two weeks of the term. The documentation of your disability must come in writing from the Accessible Education Center in the Office of Academic Advising and Student Services.  Disabilities may include (but are not limited to) neurological impairment, orthopedic impairment, traumatic brain injury, visual impairment, chronic medical conditions, emotional/psychological disabilities, hearing impairment, and learning disabilities. For more information on Accessible Education Center, please see http://aec.uoregon.edu 

## Mandatory Reporting of Child Abuse
UO employees, including faculty, staff, and GEs, are mandatory reporters of child abuse. This statement is to advise you that that your disclosure of information about child abuse to a UO employee may trigger the UO employee’s duty to report that information to the designated authorities. Please refer to the following links for detailed information about mandatory reporting:
http://hr.uoregon.edu/policies-leaves/general-information/mandatory-reporting-child-abuse-and-neglect

## Reporting Title IX Experiences
Any student who has experienced sexual assault, relationship violence, sex or gender-based bullying, stalking, and/or sexual harassment may seek resources and help at safe.uoregon.edu. To get help by phone, a student can also call either the UO’s 24-hour hotline at 541-346-7244 [SAFE], or the non-confidential Title IX Coordinator at 541-346-8136. From the SAFE website, students may also connect to Callisto, a confidential, third-party reporting site that is not a part of the university. 

Students experiencing any other form of prohibited discrimination or harassment can find information at aaeo.uoregon.edu or contact the non-confidential AAEO office at 541-346-3123 or the Dean of Students Office at 541-346-3216 for help. As UO policy has different reporting requirements based on the nature of the reported harassment or discrimination, additional information about reporting requirements for discrimination or harassment unrelated to sexual assault, relationship violence, sex or gender based bullying, stalking, and/or sexual harassment is available at http://aaeo.uoregon.edu/content/discrimination-harassment 

Specific details about confidentiality of information and reporting obligations of employees can be found at https://titleix.uoregon.edu. 

## Academic Misconduct Policy
All students are subject to the regulations stipulated in the UO Student Conduct Code http://conduct.uoregon.edu). This code represents a compilation of important regulations, policies, and procedures pertaining to student life. It is intended to inform students of their rights and responsibilities during their association with this institution, and to provide general guidance for enforcing those regulations and policies essential to the educational and research missions of the University.  

## Conflict Resolution 
Several options, both informal and formal, are available to resolve conflicts for students who believe they have been subjected to or have witnessed bias, unfairness, or other improper treatment. 

It is important to exhaust the administrative remedies available to you including discussing the conflict with the specific individual, contacting the Department Head, or within the College of Education, you can contact the Associate Dean for Academic Affairs and Equity (Krista Chronister, 346-2415, kmg@uoregon.edu). Outside the College, you can contact: 
* UO Bias Response Team: 346-3216 http://bias.uoregon.edu/whatbrt.htm 
* Affirmative Action and Equal Opportunity: 346-3123 http://aaeo.uoregon.edu/

## Grievance Policy
A student or group of students of the College of Education may appeal decisions or actions pertaining to admissions, programs, evaluation of performance and program retention and completion. Students who decide to file a grievance should follow the student grievance procedure, or alternative ways to file a grievance outlined in the Student Grievance Policy (https://education.uoregon.edu/academics/student-grievance) or enter search: student grievance.

## In Case of Inclement Weather 
In the event the University operates on a curtailed schedule or closes, UO media relations will notify the Eugene-Springfield area radio and television stations as quickly as possible. In addition, a notice regarding the university’s schedule will be posted on the UO main home page (in the “News” section) at http://www.uoregon.edu. Additional information is available at http://hr.uoregon.edu/policy/weather.html.

If an individual class must be canceled due to inclement weather, illness, or other reason, a notice will be posted on Canvas or via email. During periods of inclement weather, please check Canvas and your email rather than contact department personnel. Due to unsafe travel conditions, departmental staff may be limited and unable to handle the volume of calls from you and others.

## Course Incomplete Policy
Students are expected to be familiar with university policy regarding grades of “incomplete” and the time line for completion. For details on the policy and procedures regarding incompletes, Please see: https://education.uoregon.edu/academics/incompletes-courses
