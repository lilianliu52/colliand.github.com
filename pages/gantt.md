---
layout: post
title:  "Learn how to use Gantt Chart"
date:   2015-05-20 
categories: support flowcharts
robots: noindex
---

<script src="https://cdnjs.cloudflare.com/ajax/libs/mermaid/0.4.0/mermaid.full.js"></script>
<link rel="stylesheet" href="{{site.baseurl}}/css/mermaid.forest.css">

<script>
        var mermaid_config = {
            startOnLoad:true
        }
        mermaid.startOnLoad = true;
        mermaid.sequenceConfig = {"diagramMarginX":50,"diagramMarginY":10,"actorMargin":50,"width":150,"height":45,"boxMargin":10,"boxTextMargin":5,"noteMargin":10,"messageMargin":35, "mirrorActors":false};
        mermaid.ganttConfig = {
            titleTopMargin:25,
            barHeight:20,
            barGap:4,
            topPadding:50,
            sidePadding:75,
            gridLineStartPadding:35,
            fontSize:11,
            numberSectionStyles:3,
            axisFormatter: [
                // Within a day
                ["%I:%M", function (d) {
                    return d.getHours();
                }],
                // Monday a week
                ["w. %U", function (d) {
                    return d.getDay() == 1;
                }],
                // Day within a week (not monday)
                ["%a %d", function (d) {
                    return d.getDay() && d.getDate() != 1;
                }],
                // within a month
                ["%b %d", function (d) {
                    return d.getDate() != 1;
                }],
                // Month
                ["%m-%y", function (d) {
                    return d.getMonth();
                }]
            ]
        };
</script>

 
### Gantt Experiment
 
<div class="mermaid">
gantt
        dateFormat  YYYY-MM-DD
        title Adding GANTT diagram functionality to mermaid

        section Changing?
        Completed task            :done,    des1, 2014-01-06,2014-01-08
        Active task               :active,  des2, 2014-01-09, 3d
        Future task               :         des3, after des2, 5d
        Future task2               :         des4, after des3, 5d

        section Critical tasks
        Completed task in the critical line :crit, done, 2014-01-06,24h
        Implement parser and jison          :crit, done, after des1, 2d
        Create tests for parser             :crit, active, 3d
        Future task in critical line        :crit, 5d
        Create tests for renderer           :2d
        Add to mermaid                      :1d

        section Documentation
        Describe gantt syntax               :active, a1, after des1, 3d
        Add gantt diagram to demo page      :after a1  , 20h
        Add another diagram to demo page    :doc1, after a1  , 48h

        section Last section
        Describe gantt syntax               :after doc1, 3d
        Add gantt diagram to demo page      : 20h
        Add another diagram to demo page    : 48h
</div>

<div class="mermaid">
        gantt
        title A Gantt Diagram
        dateFormat  YYYY-MM-DD
        section Section
        A task           :a1, 2015-01-01, 3d
        Another task     :after a1  , 20d
        section Another
        Task in sec      :2015-01-12  , 12d
        section Another2
        anther task      : 40d
        section Another3
        anther task      : 24d
        section Another4
        anther task      : 33d
        section Another5
        anther task      : 24d
        section Another6
        anther task      : 41d
        section Another7
        anther task      : 24d
        section Another8
        anther task      : 24d
        section Another9
        anther task      : 31d
        anther task      : 2d
        section Another10
        anther task      : 36d
        section Another11
        anther task      : 36d
        section Another12
        anther task      : 37d
</div>