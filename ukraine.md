---
layout: post-layout
title: FLOWStandsWithUkraine
description: FLOW's team is deeply concerned about the recently fueled war in Ukraine. We dedicate our efforts to raise awareness regarding the gravity of this war and its implications for international security.
image: ../img/ukraine-flag.webp
date: 26 December 2022
navbar-class: navbar-ukraine
content-class: wide-9
text-center: true
---

## Discussion Panel on **"The War in Ukraine: Implications on International Security"**

FLOW's Co-founder and CEO organized and moderated the discussion with the
participation of regional experts at the <a class="nice-link" href="https://korbel.du.edu/academics-degrees/graduate-degrees?gclid=Cj0KCQiA95aRBhCsARIsAC2xvfz8BU6Ti-G4xmciO98dqHWQZVX9BY1pEfGjQgqSCl48oh3Q9vENDQIaAlPOEALw_wcB"
target="blank_">Josef Korbel School of
International Studies</a>, University of Denver.

The discussion was supported by Professor Steve Recca of the Korbel School
and Ambassador of Georgia to the Republic of Bulgaria & North Macedonia
Tamara Liluashvili

<div class="container-fluid">
    <div class="row no-gutter justify-content-center text-center">
        {% for participant in site.data.ukraine-war %}
            <div class="col-lg-4 col-sm-6 center-block">
                <div style="min-height: 350px">
                    <img src="img/ukraine/{{ participant.img }}" class="img-responsive participant-img ukraine-grid-img">
                    <p class="participant-name">{{ participant.name }}</p>
                    <p class="participant-desc">{{ participant.desc }}</p>
                </div>
            </div>
        {% endfor %}
    </div>
</div>
