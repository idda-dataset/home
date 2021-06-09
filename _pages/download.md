---
permalink: /download/
layout: splash
toc: false
author_profile: true
title: "Download"
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/download.jpg
---

<script>
function myFunction() {
  var x = document.getElementById("mySelect").value;
  if (x == "yes"){
    document.getElementById("ifYes").style.display = "none";
  }else if (x == ""){
    document.getElementById("ifYes").style.display = "none";
  }else{
    document.getElementById("ifYes").style.display = "block";
  }
}
</script>

<div style="word-wrap: break-word; width:auto; margin: auto; padding: 16px; box-shadow: 5px 5px 5px 5px #CCCCCC;" >

<form accept-charset="UTF-8" action="https://getform.io/f/da0906d1-21bc-42cc-ba85-6dc77904a443" method="POST" enctype="multipart/form-data" target="_blank">
  <fieldset>
    <legend><b>Compile this form to request the splitting used in the IDDA paper</b></legend>
    <p><br><br><br></p>
    <label for="fname">Name*:</label><br>
    <input type="text" id="fname" style="border: none; border-bottom: 0.01em solid gray;" required><br>
    <label for="lname">Surname*:</label><br>
    <input type="text" id="lname" style="border: none; border-bottom: 0.01em solid gray;" required><br>
    <label for="email">Email*:</label><br>
    <input type="email" id="email" style="border: none; border-bottom: 0.01em solid gray;" required><br>
    <label for="company">Organization:</label><br>
    <input type="text" id="company" style="border: none; border-bottom: 0.01em solid gray;"><br>
    <label for="reason">Reason for use of dataset*:</label><br>
    <textarea id="reason" style="border: none; border-bottom: 0.01em solid #808080;" rows="5" required></textarea><br>
    <input type="checkbox" id="best" name="best" value="Splitting Best"> <label for="best"> Splitting Best </label><br>
    <input type="checkbox" id="worst" name="worst" value="Splitting Worst"> <label for="worst"> Splitting Worst </label><br>
    <input type="checkbox" id="t01csa" name="t01csa" value="T01 CS A"> <label for="t01csa"> T01 CS A </label><br>
    <input type="submit" value="Request" class="btn--info"/>
  </fieldset>
</form>
</div>
<br>
<br>
<br>

*Required field<br>
Dataset download will be available next week.
{: .notice--warning}