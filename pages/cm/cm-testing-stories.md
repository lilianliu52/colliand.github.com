---
layout: post
title:  "Crowdmark Testing Stories"
date:   2015-05-05
categories: crowdmark testing flowcharts
robots: noindex
comments: false
---

<script src="https://cdn.rawgit.com/knsv/mermaid/0.4.0/dist/mermaid.full.js"></script>




## 0. Setup X User Contexts

**Roles**  

* Student
* Uploader
* Grader
* Facilitator
* Owner

**Browsers**

* Chrome
* Firefox
* IE
* Safari

**Operating Systems**

* Apple
* Linux
* Windows


**Crowdmark Configuration**

* LTI
* Stand-alone

Our testing should explore the **Roles X Browsers X Operating Systems X Configuration** space of contexts.


***
***


## 1. Assigned Assessment Creation Testing List

<div class="mermaid">
graph TB
    A((Start)) -->|1. Enter Title| B{2. Select Type}
    B -->|3. Assigned| H(Template)
    H -->|4. Upload Template| I(Details)
    I -->|5. Due Date<br>6. Lateness Penalty<br>7. Optional Note| J(Enrollments)
    J -->|8. Enter Emails| K(Distribute)
    K -->|9. Click to send| G(10. Dashboard)
    style A fill:#8bc341,stroke:#333,stroke-width:2px;
    style G fill:#8bc341,stroke:#333,stroke-width:2px;
    style B fill:#0091d6,stroke:#333,stroke-width:2px;
    style H fill:#bd5a9b,stroke:#333,stroke-width:2px;
    style J fill:#009bc7,stroke:#333,stroke-width:2px;
  
</div>

***

1. Type *title* in `New Assessment Name` Field
2. Select type `Assigned` (see `Administered` in Section 2.)
3. Click to start Assigned Wizard
4. Upload *assigned template*
5. Enter `Due Date`
6. Enter `Lateness Penalty`
7. Enter `Optional Note` to include with assigned email invitations
8. Enter *email addresses*
9. Distribute assigned emails
10. Click to return to Dashboard

***
***

## 2. Administered Assessment Creation Testing List

<div class="mermaid">
graph TB
    A((Start)) -->|1. Enter Title| B{2. Select Type}
    B -->|3. Administered| D(Template)
    D ---|4. Double-sided?<br>5. Single-sided?<br>6. Upload Template| E(Enrollments)
    E -->|7. Enter Emails<br>8. Extra Assessments?| F(Generate PDF)
    F -->|9. Download PDF<br>10. Return to Dashboard| G((Dashboard))
    style A fill:#8bc341,stroke:#333,stroke-width:2px;
    style G fill:#8bc341,stroke:#333,stroke-width:2px;
    style B fill:#0091d6,stroke:#333,stroke-width:2px;
    style D fill:#bd5a9b,stroke:#333,stroke-width:2px;
    style E fill:#009bc7,stroke:#333,stroke-width:2px;
</div>

***

1. Type *title* in `New Assessment Name` Field
2. Select type `Administered` (see `Assigned` in Section 1.)
3. Click to start Administered Wizard
4. Toggle radio button to select `double-sided` 
5. Toggle radio button to select `single-sided` (Repeat entire workflow.)
6. Upload *administered template*
7. Enter *email addresses*
8. Select *number* of extra assessments
9. Download printable PDF file
10. Click to return to Dashboard

***
***

## 3. how to grade testing list
 
<div class="mermaid">
graph TB
    A(Dashboard) -->|1. Click| B(Start Grading)
    B --> C>Grading Grid] 
    C -->|2. Click| E(Grading tips)
    E -->|Read tips<br>|G(3. Click closes tips)
    C -->|4. Click| F[Question Tile]
    F --> H((Grading Interface))
    H -->|5. Click or 6. z|J(Pen Mode)
    J --> K(7. Press mouse<br>down to draw)
    H -->|9. Click or 10. V|L(Comment Mode)
    H -->|14. Click or 15. x| M(X Mode)
    H -->|17. Click or 18. c| N(Check Mode)
    H -->|20. Keypad or 21. numbers| O(Enter Score)
    J -->|8. double-click|L
    L -->|11. Click| P(12. Markdown/13. Mathjax<br>comment text)
    M -->|16. Click| Q(Drop X)
    N -->|19. Click| R(Drop Checkmark)
    style A fill:#867cb8,stroke:#333,stroke-width:0px;
    style B fill:#8bc341,stroke:#333,stroke-width:0px;
    style E fill:#ccf,stroke:#f66,stroke-width:2px,stroke-dasharray: 5, 5;
    style H fill:#aa5f9f,stroke:#333,stroke-width:0px;
    style J fill:#40a8c3,stroke:#333,stroke-width:0px;
    style M fill:#40a8c3,stroke:#333,stroke-width:0px;
    style N fill:#40a8c3,stroke:#333,stroke-width:0px;
    style O fill:#40a8c3,stroke:#333,stroke-width:0px;
    style L fill:#40a8c3,stroke:#333,stroke-width:0px;
    
 
</div>


1. Click `Start Grading` Button
2. Click `Grading tips` button
3. Click to close tips
4. Click `Question tile` to enter Grading Interface
5. Test Pen Mode entry with *z*
6. Test pen Mode entry with *click on pen*
7 Press mouse down to draw in pen mode
8. Test double-click to enter comment box
9. Test Comment Mode entry with *click*
10. Test Comment Mode entry with *v*
11. Click to open text box
12. Enter *Markdown* to test markdown parsing
13. Enter *TeX* to test Mathjax parsking
14. Test X mode entry with click
15. Test X mode entry with *x*
16. Test drop of X with click
17. Test Checkmark mode entry with click
18. Test Checkmark mode entry with *c*
19. Test drop of Checkmark with click


***
***

## 4. Hover States in Grading Interface testing list

<div class="mermaid">
graph TB
    A>Grading Grid] -->|1. hover| B[Question Tile]
    A -->|2. hover| C(Grader Avatar)
    style B stroke:#333,stroke-width:2px;
 
</div>

***

1. Confirm email hover tip on grading team `avatars`.
2. Confirm email hover tip behavior on `question tiles`. (Graders don't see anything, facilitators see email hover tip. Depends on whether the assessment containing the tile has been matched to a student's identity.)

***
***


## 5.  Add student metadata testing list
 
<div class="mermaid">
graph TB
    A(Dashboard) -->|1. Click| B(Students)
    B -->|2. Click| D(Upload metadata)
    D -->|3. Select CSV file| B
    style A fill:#867cb8,stroke:#333,stroke-width:2px;
    style B stroke:#333,stroke-width:2px;
    style D fill:#40a8c3,stroke:#333,stroke-width:2px;
 
</div>

***

1. Click to enter `Students`
2. Click the button to Upload metadata
3. Select *CSV file with student metatdata*

***
***


## 6. Invite Grading Team Testing List
 
<div class="mermaid">
graph TB
    A(Dashboard) -->|1. Click| B(Grading Team)
    B -->|2. Click| D(+ Invite)
    D ---|3. Enter Emails<br>4. Select Role<br>5. Click| E(Invite)
    E --> B
    style A fill:#867cb8,stroke:#333,stroke-width:2px;
    style B stroke:#333,stroke-width:2px;
    style D fill:#40a8c3,stroke:#333,stroke-width:2px;
    style E fill:#009bc7,stroke:#333,stroke-width:2px;
</div>

***

1. Click to enter `Grading Team`
2. Click `+ Invite`
3. Enter *Emails for new team members*
4. Select *role* for new team members
5. Click `Invite`

***
***

## 7. Saving of Evaluations Testing List

collisions  
next ungraded  
order of operations  
cancel score  
multiple evaluations??  
deletion of comments 
deletion of annotations

***
***

## 8. Export Scores File as CSV Testing List



***
***
## 9. Results Section Testing List


***
***
## 10. Delete Assessment Testing List


***
***
## 11. Question Setup Testing List


***
***
## 12. Send Grades to Students


***
***
## 13. Student Upload Assigned Testing List


***
***
## 14. Student Receives Scores Email Testing List


***
***
## 15. Upload Assessments Testing List


***
***
## 16. Fix Scan Errors Testing List


***
***
## 17. Resend Assigned Assessment Invitation Email Testing List


***
***
## 18. Send Support Message Using Envelope Icon Testing list


***
***
## 19. Access Support Knowledge Base with Question Mark Icon Testing List
