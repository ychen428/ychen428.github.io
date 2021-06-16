---
layout: page
permalink: /
title: about
nav: about
description: <a href="https://lsa.umich.edu/chem" class="page-description" target="_blank">Chemistry Department</a> • <a href="https://rackham.umich.edu/" class="page-description" target="_blank">Rackham Graduate School</a> • <a href="https://umich.edu/" class="page-description" target="_blank">University of Michigan, Ann Arbor</a>
---

<div class="col p-0 pt-4 pb-4">
  <h1 class="pb-3 title text-left font-weight-bold">Yuting Chen</h1>
  <h6 class="m-0 mb-2" style="font-size: 0.83em;">{{ page.description }}</h6>
  {% if page.address %}
      <h6 class="m-0 mb-2" style="font-size: 0.83em;">{{ page.address }}</h6>
  {% endif %}
</div>

<!-- Introduction -->

<div style="display: flex; flex-wrap: wrap;">
    <div class="text-justify p-0">
        <div class="col-xs-12 col-sm-6 p-0 pt-2 pb-sm-2 pb-4 pl-sm-4 text-center" style="float: right;">
          <img class="profile-img img-responsive" src="{{ 'penguin.png' | prepend: '/assets/img/' | prepend: site.baseurl | prepend: site.url }}">
        </div>

        <p>
            I am a Ph.D. student in the <a href="https://lsa.umich.edu/chem" class="page-description" target="_blank">Chemistry Department</a>  at <a href="https://umich.edu/" class="page-description" target="_blank">University of Michigan, Ann Arbor</a>, advised by <a href="https://lsa.umich.edu/chem/people/faculty/zgid.html" target="_blank">Dominika Zgid</a>.
        <p>
            My Ph.D. research focuses on developing algorithms quantum chemistry simulations. Under Construction
        <p>
            Before I joined UMich, I graduated with an B.S. in Chemistry and a minor in Computer Science from the <a href="https://www.berkeley.edu/" target="_blank">University of California, Berkeley</a>.
            There I worked with <a href="https://mhggroupberkeley.com/" target="_blank">Martin Head-Gordon</a> and <a href="https://simons.berkeley.edu/people/alec-white" target="_blank">Alec White</a> to develop better initial guesses for SCF iterations.
        </p>
  </div>
</div>


<!-- News -->
<div class="news mt-3 p-0">
  <h1 class="title mb-4 p-0">news</h1>
  {% assign news = site.news | reverse %}
  {% for item in news limit: site.news_limit %}
    <div class="row p-0">
      <div class="col-sm-2 p-0">
        <span class="badge light-green darken-1 font-weight-bold text-uppercase align-middle date ml-3">
          {{ item.date | date: "%b %-d, %Y" }}
        </span>
      </div>
      <div class="col-sm-10 mt-2 mt-sm-0 ml-3 ml-md-0 p-0 font-weight-light text">
        <p>{{ item.content | remove: '<p>' | remove: '</p>' | emojify }}</p>
      </div>
    </div>
  {% endfor %}
</div>
