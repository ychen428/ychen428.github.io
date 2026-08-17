---
layout: default
title: contact
permalink: /contact
nav: true
nav_order: 6
timeline:
  - "7:00 AM"
  - "7:30 AM"
  - "8:00 AM"
  - "8:30 AM"
  - "9:00 AM"
  - "9:30 AM"
  - "10:00 AM"
  - "10:30 AM"
  - "11:00 AM"
  - "11:30 AM"
  - "12:00 PM"
  - "12:30 PM"
  - "1:00 PM"
  - "1:30 PM"
  - "2:00 PM"
  - "2:30 PM"
  - "3:00 PM"
  - "3:30 PM"
  - "4:00 PM"
  - "4:30 PM"
  - "5:00 PM"
  - "5:30 PM"
schedule:
  - name: Monday
    events:
      - name: Lecture
        start: 12:00 PM
        end: 2:00 PM
        location: Baker 366
  - name: Tuesday
    events:
      - name: Lecture
        start: 8:00 AM
        end: 11:00 AM
        location: Baker 338
      - name: Office Hours
        start: 4:00 PM
        end: 5:00 PM
        location: Baker Hufflepuff
  - name: Wednesday
    events:
      - name: Lecture
        start: 12:00 PM
        end: 2:00 PM
        location: Baker 366
      - name: Office Hours
        start: 4:00 PM
        end: 6:00 PM
        location: Baker Hufflepuff
  - name: Thursday
    events:
      - name: Lecture
        start: 8:00 AM
        end: 11:00 AM
        location: Baker 338
      - name: Office Hours
        start: 3:00 PM
        end: 5:00 PM
        location: Baker Hufflepuff
  - name: Friday
    events:
      - name: Lecture
        start: 12:00 PM
        end: 2:00 PM
        location: Baker 366
      - name: Office Hours
        start: 4:00 PM
        end: 5:00 PM
        location: Baker Hufflepuff
---

<style>
  .contact-card {
    border: 1px solid var(--global-divider-color);
    border-radius: 12px;
    padding: 1rem 1.25rem;
    margin: 1.5rem 0;
    background: var(--global-bg-color);
    color: var(--global-text-color);
  }

  .schedule {
    overflow-x: scroll;
    position: relative;
    border: 1px solid var(--global-divider-color);
    border-radius: 12px;
    padding: 1rem;
    background: var(--global-bg-color);
    color: var(--global-text-color);
  }
  .schedule li::before {
    display: none;
  }
  .schedule ul.schedule-timeline,
  .schedule ul.schedule-group,
  .schedule ul.schedule-events {
    margin-top: 0;
    padding-left: 0;
  }
  .schedule ul.schedule-timeline {
    margin: 40px auto 0;
    position: absolute;
    width: 100%;
  }
  .schedule .schedule-time {
    color: var(--global-text-color-light, var(--global-text-color));
    height: 40px;
    margin: 0;
    padding: 0.5rem;
    position: relative;
    font-size: 0.8rem;
    list-style: none;
  }
  .schedule .schedule-time::after {
    background-color: var(--global-divider-color);
    content: "";
    height: 1px;
    left: 0;
    position: absolute;
    top: 0;
    width: 100%;
  }
  .schedule .schedule-group {
    display: flex;
    margin-bottom: 0;
    position: relative;
  }
  .schedule .schedule-day {
    border-left: 1px solid var(--global-divider-color);
    flex: 1 0 0;
    margin: 0;
    min-width: 140px;
    list-style: none;
  }
  .schedule .schedule-day:first-of-type {
    border-left: 0;
  }
  .schedule h2.schedule-header {
    align-items: center;
    display: flex;
    font-size: 18px;
    height: 40px;
    justify-content: center;
    margin: 0;
    color: var(--global-text-color);
  }
  .schedule .schedule-events {
    display: flex;
    padding: 0;
    position: relative;
  }
  .schedule .schedule-event {
    border-radius: 8px;
    float: left;
    height: 100%;
    margin: 0;
    padding: 0.5rem;
    position: absolute;
    width: calc(100% - 8px);
    left: 4px;
    box-sizing: border-box;
    overflow: hidden;
  }
  .schedule .schedule-event .name {
    font-weight: 700;
    font-size: 0.95rem;
  }
  .schedule .schedule-event .time,
  .schedule .schedule-event .location {
    font-size: 0.8rem;
  }

  /* Light mode (default) - pastel tones with dark text for contrast */
  .schedule .schedule-event {
    color: #1a1a1a;
    box-shadow:
      0 10px 20px rgba(0, 0, 0, 0.05),
      inset 0 -3px 0 rgba(0, 0, 0, 0.08);
  }
  .schedule .schedule-event.drop-in {
    background-color: #d1d5db; /* grey */
  }
  .schedule .schedule-event.lecture,
  .schedule .schedule-event.lab {
    background-color: #93c5fd; /* blue */
  }
  .schedule .schedule-event.problem-solving {
    background-color: #d8b4fe; /* purple */
  }
  .schedule .schedule-event.office-hours {
    background-color: #fcd34d; /* amber */
  }

  /* Dark mode - richer/saturated tones with light text */
  html[data-theme="dark"] .schedule .schedule-event {
    color: white;
    box-shadow:
      0 10px 20px rgba(0, 0, 0, 0.2),
      inset 0 -3px 0 rgba(0, 0, 0, 0.2);
  }
  html[data-theme="dark"] .schedule .schedule-event.drop-in {
    background-color: #4b5563;
  }
  html[data-theme="dark"] .schedule .schedule-event.lecture,
  html[data-theme="dark"] .schedule .schedule-event.lab {
    background-color: #2563eb;
  }
  html[data-theme="dark"] .schedule .schedule-event.problem-solving {
    background-color: #7c3aed;
  }
  html[data-theme="dark"] .schedule .schedule-event.office-hours {
    background-color: #b45309;
  }
</style>

## Current Students

There are a few ways to reach me:

* Email: I generally reply within 24 hours, Monday to Friday. If you email me over the weekend, I won't see your email until Monday.

* Course Content Questions: For questions related about the material, please post your question to the discussion board on Labpal or come to office hours in Baker.

* Personal Office Hours: For one-on-one meetings to discuss something specific to your situation in private (class performance, grades, accomdations, college life, anything else you want discuss one-on-one) please make an appointment via email.

<!-- * Drop in Office Hours: In the schedule below I've highlighted my availability for drop in. If the door is open and I'm in, feel free to pop in. -->
<!-- <button data-cal-link="yuting-hamilton/15min" data-cal-namespace="15min" data-cal-config='{"layout":"month_view","useSlotsViewOnSmallScreen":"true"}'>Schedule a meeting</button>

<script type="text/javascript">
  (function (C, A, L) { let p = function (a, ar) { a.q.push(ar); }; let d = C.document; C.Cal = C.Cal || function () { let cal = C.Cal; let ar = arguments; if (!cal.loaded) { cal.ns = {}; cal.q = cal.q || []; d.head.appendChild(d.createElement("script")).src = A; cal.loaded = true; } if (ar[0] === L) { const api = function () { p(api, arguments); }; const namespace = ar[1]; api.q = api.q || []; if(typeof namespace === "string"){cal.ns[namespace] = cal.ns[namespace] || api;p(cal.ns[namespace], ar);p(cal, ["initNamespace", namespace]);} else p(cal, ar); return;} p(cal, ar); }; })(window, "https://app.cal.com/embed/embed.js", "init");
  Cal("init", "15min", {origin:"https://app.cal.com"});
  Cal.config = Cal.config || {};
  Cal.config.forwardQueryParams = true;
  Cal.ns["15min"]("ui", {"hideEventTypeDetails":false,"layout":"month_view"});
</script> -->

## Former Students

Always happy to hear from former students, shoot me an email (ychen56@calpoly.edu) anytime, whether it's to just say hi, catch up, or ask for advice.

## General Availability

{% assign start_time = page.timeline | first %}
{% capture offset %}{% include minutes.liquid time=start_time %}{% endcapture %}
<div class="schedule">
  <ul class="schedule-timeline">
    {% for time in page.timeline %}
    <li class="schedule-time">{{ time }}</li>
    {% endfor %}
  </ul>
  <ul class="schedule-group">
    {% for day in page.schedule %}
    <li class="schedule-day">
      <h2 class="schedule-header">{{ day.name }}</h2>
      {% if day.events %}
      <ul class="schedule-events" style="height: {{ page.timeline | size | times: 40 }}px">
        {% for event in day.events %}
        {% capture start %}{% include minutes.liquid time=event.start %}{% endcapture %}
        {% capture end %}{% include minutes.liquid time=event.end %}{% endcapture %}
        {% assign top = start | minus: offset | times: 40 | divided_by: 30 %}
        {% assign height = end | minus: start | times: 40 | divided_by: 30 %}
        <li class="schedule-event {{ event.name | slugify }}" style="top: {{ top }}px; height: {{ height }}px;">
          <div class="name">{{ event.name }}</div>
          <div class="time">{{ event.start }}–{{ event.end }}</div>
          {% if event.location %}
          <div class="location">{{ event.location }}</div>
          {% endif %}
        </li>
        {% endfor %}
      </ul>
      {% endif %}
    </li>
    {% endfor %}
  </ul>
</div>