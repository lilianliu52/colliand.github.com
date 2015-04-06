---
author: James Colliander
title: flowchart
excerpt:
layout: page
<!-- permalink: /calculus/ -->
robots: noindex
---


<script src="https://cdn.rawgit.com/knsv/mermaid/0.3.0/dist/mermaid.full.js"></script>



### Crowdmark Assessment Creation

<div class="mermaid">
graph TB
    A((Start)) -->|Enter Title| B{Select Type}
    B -->|Administered| D(Template)
    B -->|Assigned| H(Template)
    D ---|Double-sided?<br>Upload Template| E(Enrollments)
    E -->|Enter Emails<br>Extra Assessments?| F(Generate PDF)
    F -->|Download PDF| G((Dashboard))
    H -->|Upload Template| I(Details)
    I -->|Due Date<br>Lateness Penalty<br>Optional Note| J(Enrollments)
    J -->|Enter Emails| K(Distribute)
    K --> G
    style A fill:#8bc341,stroke:#333,stroke-width:2px;
    style G fill:#8bc341,stroke:#333,stroke-width:2px;
    style B fill:#0091d6,stroke:#333,stroke-width:2px;
    style H fill:#bd5a9b,stroke:#333,stroke-width:2px;
    style D fill:#bd5a9b,stroke:#333,stroke-width:2px;
    style J fill:#009bc7,stroke:#333,stroke-width:2px;
    style E fill:#009bc7,stroke:#333,stroke-width:2px;
</div>


 
### How to grade?
 
<div class="mermaid">
graph TB
    A(Dashboard) -->|Click| B(Start Grading)
    B --> C>Grading Grid] 
    C -->|Click| E(Grading tips)
    E -->|Read tips<br>|G(Click closes tips)
    C -->|Click| F[Question Tile]
    F --> H((Grading Interface))
    H -->|z or Click|J(Pen Mode)
    J --> K(Press mouse<br>down to draw)
    H -->|Click or V|L(Comment Mode)
    H -->|Click or x| M(X Mode)
    H -->|Click or c| N(Check Mode)
    H -->|Keypad or numbers| O(Enter Score)
    J -->|double-click|L
    L -->|Click| P(Markdown/Mathjax<br>comment text)
    M -->|Click| Q(Drop X)
    N -->|Click| R(Drop Checkmark)
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


 
### Add student metadata
 
<div class="mermaid">
graph TB
     A(Dashboard) -->|Click| B(Students)
    B -->|Click| D(Upload metadata)
    D -->|Select CSV file| B
    style A fill:#867cb8,stroke:#333,stroke-width:2px;
    style B stroke:#333,stroke-width:2px;
    style D fill:#40a8c3,stroke:#333,stroke-width:2px;
 
</div>


### Invite Grading Team
 
<div class="mermaid">
graph TB
     A(Dashboard) -->|Click| B(Grading Team)
    B -->|Click| D(&#8853 Invite)
    D ---|Enter Emails<br>Select Role<br>Click| E(Invite)
    E --> B
    style A fill:#867cb8,stroke:#333,stroke-width:2px;
    style B stroke:#333,stroke-width:2px;
    style D fill:#40a8c3,stroke:#333,stroke-width:2px;
    style E fill:#009bc7,stroke:#333,stroke-width:2px;
</div>


