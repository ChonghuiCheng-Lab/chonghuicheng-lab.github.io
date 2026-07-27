---
layout: profiles
permalink: /team/
title: team
description: members of the Cheng Lab
nav: true
nav_order: 2

profiles:
  # if you want to include more than one profile, just replicate the following block
  # and create one content file for each profile inside _pages/
  # Principal Investigator
  - align: right
    image: prof_pic.jpg
    content: about_einstein.md # TODO: replace with a real PI bio content file
    image_circular: false # crops the image to make it circular
    more_info: >
      <p>Chonghui Cheng, M.D., Ph.D. — Professor, Principal Investigator</p>
      <p>Room N1110.02, MS: BCM600</p>
      <p>Houston, TX 77030</p>
---

## Lab Members

<style>
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
    </figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/lab_members/patel-khushali-6583e41e9fe3.png' | relative_url }}" alt="Khushali Patel">
    <figcaption>
      <div class="member-name">Khushali Patel</div>
      <div class="member-role">Graduate Student</div>
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
    <img src="{{ '/assets/img/lab_members/wang-ying-ac6bb9d522ac.jpeg' | relative_url }}" alt="Ying Wang">
    <figcaption>
      <div class="member-name">Ying Wang</div>
    </figcaption>
  </figure>
</div>
