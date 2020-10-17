---
title: "Write to me"
permalink: "/contact-form/"
classes:
  - wide
sidebar:
  nav: "docs"
---

<!-- <link rel="stylesheet" href="{{ site.url }}{{ site.baseurl }}/custom-css/contact-form.css"> -->
<style>
  .container-cf {
    margin: 0;
}

.container-cf progress {
  width: 100%;
}
input {
  transition: all 0.5s;
}
</style>
<div class="notice--info">
  <h3 style="color: rgb(45, 45, 180)">Open to job opportunities:</h3><br>
  <ul style="font-size:1em; color: rgb(49, 49, 138);">
    <li>Postdoctoral Researcher (Computational geophysics)</li>
    <li>Data Analyst/Scientist</li>
    <li>Web Developer [Full-stack]</li>
  </ul>
  <a href = "mailto: utpalkumar@gate.sinica.edu.tw" style="font-size:0.6em"> <i class="fas fa-paper-plane" style="font-size: larger;"></i> Email me (with your default mail client)</a>
  </div>

<link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap.min.css'>
<div class="container-cf">
  <form onsubmit="sendEmail(event)" style="padding: 0;">
    <div id="alert-field" class="alert hidden">
      <p>Uh oh! Something went wrong!</p>
    </div>    
    <div class="form-group col-xs-6">
      <label for="name-field">Name</label>
      <input type="text" class="form-control" id="name-field" name="name-field" placeholder="Your name" required>
    </div>
    
  <div class="form-group col-xs-6">
    <label for="email-field">Email</label>
    <input type="email" class="form-control" id="email-field" name="email-field" placeholder="Email address" required>
  </div>
  
  <div id="subject-select" class="form-group col-xs-12">
    <label for="subject-field">Subject</label>
    <select class="form-control" name="subject-field" onchange="changeSubject(event)"  required>
      <option value="JobOpportunity">Post-doctorate Opportunity</option>
      <option value="Web Development">Web Development Projects</option>
      <option value="Data Scientist Opportunity">Data Scientist Opportunity</option>
      <option value="Other">Other</option>
    </select>
  </div>
  
  <div id="hidden-other-subject" class="form-group col-xs-6 hidden">
    <label for="other-subject-field">Other</label>
    <input type="text" class="form-control" id="other-subject-field" name="other-subject-field" placeholder="Other subject" />
  </div>
  
  <div class="form-group col-xs-12">
    <label for="body-field">Message</label>
    <textarea id="body-field" name="body-field" class="form-control" placeholder="Type your message here" required></textarea>
  </div>
  
  <div class="form-group col-xs-12">
    <button type="submit" class="btn btn-primary btn-lg btn-block">Submit</button>  
  </div>
    
  </form>
</div>
<!-- partial -->
  <script src='https://cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js'></script>
  <script  src="{{ site.url }}{{ site.baseurl }}/custom-js/contactForm.js"></script>


