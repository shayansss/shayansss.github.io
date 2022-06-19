---
layout: archive
title: "Professional Experience"
permalink: /experience/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}





<style type="text/css">
        :root {
  --primary-color: #ffffff;
  --background-color: rgb(255, 255, 255);
  --font: sans-serif;
}

* {
  margin: 0;
  padding: 0;
}

body {
  background: var(--background-color);
  font-family: var(--font);
  display: flex;
  justify-content: center;
}

/* Timeline Container */
.timeline {
  background: var(--primary-color);
  margin: 20px auto;
  padding: 20px;
}

/* Card container */
.card {
  position: relative;
  max-width: 400px;
}

/* setting padding based on even or odd */
.card:nth-child(odd) {
  padding: 30px 0 30px 30px;
}
.card:nth-child(even) {
  padding: 30px 30px 30px 0;
}
/* Global ::before */
.card::before {
  content: "";
  position: absolute;
  width: 50%;
  border: solid orangered;
}

/* Setting the border of top, bottom, left */
.card:nth-child(odd)::before {
  left: 0px;
  top: -4.5px;
  bottom: -4.5px;
  border-width: 5px 0 5px 5px;
  border-radius: 50px 0 0 50px;
}

/* Setting the border of top, bottom, right */
.card:nth-child(even)::before {
  right: 0;
  top: 0;
  bottom: 0;
  border-width: 5px 5px 5px 0;
  border-radius: 0 50px 50px 0;
}

/* Removing the border if it is the first card */
.card:first-child::before {
  border-top: 0;
  border-top-left-radius: 0;
}

/* Removing the border if it is the last card  and it's odd */
.card:last-child:nth-child(odd)::before {
  border-bottom: 0;
  border-bottom-left-radius: 0;
}

/* Removing the border if it is the last card  and it's even */
.card:last-child:nth-child(even)::before {
  border-bottom: 0;
  border-bottom-right-radius: 0;
}

/* Information about the timeline */
.info {
  display: flex;
  flex-direction: column;
  background: #333;
  color: gray;
  border-radius: 10px;
  padding: 10px;
}

/* Title of the card */
.title {
  color: orangered;
  position: relative;
}

/* Timeline dot  */
.title::before {
  content: "";
  position: absolute;
  width: 10px;
  height: 10px;
  background: white;
  border-radius: 999px;
  border: 3px solid orangered;
}

/* text right if the card is even  */
.card:nth-child(even) > .info > .title {
  text-align: right;
}

/* setting dot to the left if the card is odd */
.card:nth-child(odd) > .info > .title::before {
  left: -45px;
}

/* setting dot to the right if the card is odd */
.card:nth-child(even) > .info > .title::before {
  right: -45px;
}
    </style>
    <div class="timeline">
  <div class="outer">
    <div class="card">
      <div class="info">
        <h3 class="title">Title 1</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. </p>
      </div>
    </div>
    <div class="card">
      <div class="info">
        <h3 class="title">Title 2</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. </p>
      </div>
    </div>
    <div class="card">
      <div class="info">
        <h3 class="title">Title 3</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. </p>
      </div>
    </div>
    <div class="card">
      <div class="info">
        <h3 class="title">Title 4</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. </p>
      </div>
    </div>
    <div class="card">
      <div class="info">
        <h3 class="title">Title 5</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. </p>
      </div>
    </div>
  </div>
</div>



## 11/2019 – Present: PhD Candidate
--------------
* Full-time
* Faculty of Computer Science, Free University of Bozen-Bolzano, Bolzano, Italy
* Implementing research projects of my PhD dissertation in return for a full scholarship.

## 09/2020 – 10/2020: Teaching Assistant (Preparatory Course in Mathematics)
--------------
* Volunteering activity
* Faculty of Computer Science, Free University of Bozen-Bolzano, Bolzano, Italy
* A presenter helping to organize a 50-hour course in the BSc program.

## 11/2016 – 07/2017: Biomedical Engineer
--------------
* Internship
* Cancer Institute, Imam Khomeini Hospital Complex, Tehran, Iran
* Physics-based (i.e., biomechanical) modeling of the cancerous tissues by Fortran user material subroutines.

## 11/2014 – 05/2015: Mechanical Engineer
--------------
* Internship
* Kimia Hajm Kish (a private engineering and designing company in building industries), Tehran, Iran
* Numerical simulation of the building structures by the stress analysis in Abaqus to find the optimum geometry and material properties.

## 03/2011 – 10/2011: Amusement Ride Supervisor
--------------
* Part-time
* Donyaye Bazi (an amusement park), Tehran, Iran
* Supervision and technical inspection of a roller coaster, cinema simulator, and bumper cars in an indoor amusement park.