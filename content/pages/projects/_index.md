---
content_type: page
description: Final project instructions and guidelines for for 6.S897 Machine Learning
  for Healthcare.
learning_resource_types:
- Projects
ocw_type: CourseSection
title: Projects
uid: 8f308296-4b99-c74b-3eca-95954f1f7ea2
---

Projects will include a proposal, poster presentation, and final report. See the list of {{% resource_link fd4248e5-f68f-2233-10cd-dc3d049961b4 "final project suggestions" %}}.

Collaboration: Students should be in groups of three registered students. Doing something related to your research is fine, but your class project should be distinct and you should be able to isolate your contributions to the project from those of any collaborators outside of the class.

Relationship to other classes: You must ask instructors for permission before submitting a project proposal if you wish to use the same project for our class and another class (it should also be stated clearly in the proposal itself). If it is one project for two classes you must:

*   Produce a project that is twice as large in depth and content as would have been required for either class individually
*   Obtain permission from the instructor of the other class
*   Moreover, all students in the project should be enrolled in both classes

Project Components
------------------

*   Project proposals (one per group)
*   Project poster presentations
*   Project report (one per group)

Proposal
--------

At most three pages, one per group. Clearly state the following:

*   Problem you wish to tackle
*   Description of data you plan to use
*   Proposed approach and methods
*   Evaluation plan
*   Timeline
*   What each student in the group will do

We understand that much of this would be preliminary at this stage, but these details are important for us to ensure that you are on the right track.

Poster Guidelines
-----------------

*   Posters should be 36” x 48”. 
*   Final project groups will be assigned in one of the two hour-long shifts. When you are not presenting, you should be learning about the final projects of your classmates.

Write-Up Guidelines
-------------------

*   You are expected to turn in a PDF of your write-up. We strongly encourage you to open source your code and submit a link to it as part of your submission (e.g. a Github repository). You should include a readme file with instruction on how to reproduce your results as well as all the data pre-processing and analysis code. Please do not include any proprietary data in your submission.
*   Each team is expected to turn in a single project report of length at most 2n+2 pages where n is the number of students in the team. References are not counted toward page limit.
*   You are required to include a section that clearly outlines the contributions of each team member.
*   You may use any template you want. If you are looking for a clear template, we recommend the {{% resource_link "f33a9ede-1abd-498a-ad9e-4feef71855bd" "MLHC template (ZIP)" %}} This file contains 1 .jpeg, 1 .tex, 1 .pdf, 1 .sty, and 1 .cls file.
*   We encourage you to include the following sections in your writeup:
    1.  _Introduction_: This section should include a brief explanation of your problem and its clinical importance. You should briefly explain your basic approach and your main conclusions. A figure is often helpful to motivate the work.
    2.  _Related work_: This section should highlight previous work related to your problem and should put your work in a broader context. It may also include a comparison of why previous approaches could not be used to solve your particular problem.
    3.  _Methods_: Here you should formally define your problem, and describe the method you implemented in detail. Include any simplifying assumptions that you make about your data or the general problem. You should enumerate any modelling choices that you had to make and justify your choices. A main figure illustrating the overall methodology often adds a lot.
    4.  _Data and experiment setup_: Include details about your data, what variables you have access to, your cohort selection criteria, and your preprocessing choices. You might find it useful to include a table with population characteristics, or an example of the data available for a specific individual, both before (i.e. the original data) and after any pre-processing (i.e. feature construction), to make the discussion concrete. Describe your benchmarks.
    5.  _Results_: Report the quantitative results of your analyses. You may choose to present graphs or tables, the important thing is that your tables and plots should summarize the relevant results that you got out of the analysis. Comment on these results: are they statistically significant? Are there interesting trends? Do you do significantly better than your benchmarks? Is there a significant treatment effect? You may also present qualitative results such as an in depth analysis of what the approach would do for a few randomly chosen patients.
    6.  _Discussion_: Highlight how your results relate to your original question formulation. Do they support your hypothesis? Do they reveal interesting insights about existing medical practices, global health outcomes, the nature of diseases, etc? Discuss limitations with your analyses and how they might motivate future research directions.