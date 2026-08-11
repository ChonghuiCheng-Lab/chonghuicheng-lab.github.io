---
layout: page
permalink: /team/
title: Team
nav: true
nav_order: 2
---

<style>
  html,
  body {
    font-family: "Open Sans", Arial, sans-serif;
    font-size: 110%;
  }
  #search-toggle .nav-link {
    font-size: 0;
  }
  #search-toggle .nav-link::before {
    content: "Search";
    font-size: 1rem;
    margin-right: 0.4em;
  }
  #search-toggle .nav-link i {
    font-size: 1rem;
  }
  .post-title {
    font-size: 40px; /* keep header text at its original (pre-150%) size */
  }
  .navbar .nav-link {
    font-size: 24px; /* keep navbar menu items at their original (pre-150%) size */
  }
  .pi-card {
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
    align-items: flex-start;
    margin-bottom: 2.5rem;
  }
  .pi-card img {
    width: 260px;
    max-width: 100%;
    aspect-ratio: 3 / 4;
    object-fit: cover;
    border-radius: 0.5rem;
    display: block;
  }
  .pi-card .pi-info p {
    margin: 0.25rem 0;
  }
  .pi-card .pi-name {
    font-weight: 600;
    font-size: 1.15em;
  }
  .lab-roster {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.75rem;
    margin-top: 1.5rem;
  }
  .lab-roster figure {
    margin: 0;
    text-align: center;
  }
  .lab-roster img {
    width: 100%;
    aspect-ratio: 1 / 1;
    object-fit: cover;
    border-radius: 0.5rem;
    display: block;
  }
  .lab-roster figcaption {
    margin-top: 0.5rem;
  }
  .lab-roster .member-name {
    font-weight: 600;
  }
  .lab-roster .member-role {
    opacity: 0.7;
    font-size: 0.9em;
  }
  @media (max-width: 768px) {
    .lab-roster {
      grid-template-columns: repeat(2, 1fr);
    }
  }
  @media (max-width: 480px) {
    .lab-roster {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="pi-card">
  <img src="{{ '/assets/img/lab_members/cheng-chonghui-e4ae06ce2a0e.jpeg' | relative_url }}" alt="Chonghui Cheng">
  <div class="pi-info">
    <p class="pi-name">Chonghui Cheng, M.D., Ph.D.</p>
    <p>Professor, Principal Investigator</p>
    <p>Room N1110.02, MS: BCM600</p>
    <p>Houston, TX 77030</p>
  </div>
</div>

## Lab Members

<div class="lab-roster">
  <figure>
    <img src="{{ '/assets/img/lab_members/bobkov-georg-9be80f4332a1.jpeg' | relative_url }}" alt="Georg Otto Milan Bobkov">
    <figcaption>
      <div class="member-name">Georg Otto Milan Bobkov</div>
      <div class="member-role">Instructor</div>
    </figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/lab_members/panici-brendan-a4b8dcc2b9d1.jpeg' | relative_url }}" alt="Brendan Panici">
    <figcaption>
      <div class="member-name">Brendan Panici</div>
      <div class="member-role">Graduate Student</div>
    </figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/lab_members/patel-khushali-6583e41e9fe3.png' | relative_url }}" alt="Khushali Patel">
    <figcaption>
      <div class="member-name">Khushali Patel</div>
      <div class="member-role">Postdoc</div>
    </figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/lab_members/wang-nicole-573293e27c81.jpeg' | relative_url }}" alt="Nicole Yiran Wang">
    <figcaption>
      <div class="member-name">Nicole Yiran Wang</div>
      <div class="member-role">MD/PhD Student (MSTP)</div>
    </figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/lab_members/michael_lee_headshot.png' | relative_url }}" alt="Michael Lee">
    <figcaption>
      <div class="member-name">Michael Lee</div>
      <div class="member-role">Graduate Student</div>
    </figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/lab_members/christian_headshot.png' | relative_url }}" alt="Christian Siangco">
    <figcaption>
      <div class="member-name">Christian Siangco</div>
      <div class="member-role">Lab technician</div>
    </figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/lab_members/pedro_headshot.png' | relative_url }}" alt="Pedro Lopez">
    <figcaption>
      <div class="member-name">Pedro Lopez</div>
      <div class="member-role">Lab technician</div>
    </figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/lab_members/Aveksha_headshot.jpg' | relative_url }}" alt="Aveksha Sharma">
    <figcaption>
      <div class="member-name">Aveksha Sharma</div>
      <div class="member-role">Postdoc</div>
    </figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/lab_members/helena_hanley_headshot.png' | relative_url }}" alt="Helena Hanley">
    <figcaption>
      <div class="member-name">Helena Hanley</div>
      <div class="member-role">Graduate Student</div>
    </figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/lab_members/yousef_headshot.jpg' | relative_url }}" alt="Yousef Khashana">
    <figcaption>
      <div class="member-name">Yousef Khashana</div>
      <div class="member-role">Graduate Student</div>
    </figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/lab_members/ruiying_headshot.png' | relative_url }}" alt="Ruiying Ma">
    <figcaption>
      <div class="member-name">Ruiying Ma</div>
      <div class="member-role">Graduate Student</div>
    </figcaption>
  </figure>
</div>
