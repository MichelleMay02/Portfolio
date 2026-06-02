+++
date = '2025-09-23T15:05:00-04:00'
draft = false
title = 'Projects'
+++

<!-- Load a cute font from Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@700;900&display=swap" rel="stylesheet">

<style>
  body {
    background-image: url("/IDP.png");
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
    font-family: 'Poppins', 'Helvetica Neue', Arial, sans-serif;
  }

  .project-container {
    display: flex;
    flex-direction: column;
    gap: 3rem;
    padding: 2rem;
    background: rgba(255,255,255,0.85);
    border-radius: 12px;
    max-width: 1200px;
    margin: auto;
  }

  /* === Logo + Description Layout === */
  .logo-bg {
    display: flex;
    flex-wrap: wrap;
    gap: 3rem;
    align-items: center;
    justify-content: center;
    padding: 3rem;
    border-radius: 12px;
    background: rgba(255, 255, 255, 1);
    text-align: center;
  }

  .logo-bg img {
    width: 550px;   
    max-width: 80%;
    border-radius: 12px;
    z-index: 1;
  }

  .logo-bg .desc {
    z-index: 1;
    font-size: 1.4rem;
    max-width: 700px;
    font-weight: 700;
    color: #008000; /* green text */
    line-height: 1.6;
  }

  /* === Google Sheet === */
  iframe {
    border: 1px solid #ccc;
    border-radius: 8px;
    width: 100%;
    height: 1000px;
    margin-top:1rem;
  }
</style>

<div class="project-container">

  <!-- Logo + Description Layout -->
  <div class="logo-bg">
    <img src="/IMPACTS.jpg" alt="Eastern Queens Alliance Logo">
    <div class="desc">
       <b>I</b>ntegrating <b>M</b>ultidisciplinary <b>P</b>ractices for <b>A</b>dvancing <b>C</b>onservation and <b>T</b>echnology in <b>S</b>ustainability
    </div>
  </div>

  <!-- Embedded Google Sheet -->
  <iframe 
      src="https://docs.google.com/spreadsheets/d/e/2PACX-1vTMHZXj8_AY7K3825sC6jX7JjQQl5IR954BDJWQ3l-KuMqK5iFPoz3PBCAYsqjw4-MhpgD5fdKXn_wd/pubhtml?widget=true&amp;headers=false">
  </iframe>

</div>
