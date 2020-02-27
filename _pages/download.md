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
  }else{
  document.getElementById("ifYes").style.display = "block";
  }
}
</script>


<form action="mailto:someone@example.com" method="post" enctype="text/plain">
  <fieldset>
    <legend>Compile this form to request the dataset or a split</legend>
    <label for="name">Name and Surname:</label><br>
    <input type="text" id="name"><br>
    <label for="email">Email:</label><br>
    <input type="email" id="email"><br>
    Do you want the whole dataset?<br>
    <select id="mySelect" onchange="myFunction();">
        <option value=""></option>
        <option value="yes">Yes</option>
        <option value="no">No</option>
    </select>
    <p id="demo"></p>
    <div id="ifYes" style="display: none;">
        <p>Create your own scenario</p><br>
        <label for="towns">Choose the town:</label><br>
        <input list="towns" name="towns">
        <datalist id="towns">
            <option value="Town 01">
            <option value="Town 02">
            <option value="Town 03">
            <option value="Town 04">
            <option value="Town 05">
            <option value="Town 06">
            <option value="Town 07">
        </datalist>
    </div>
  </fieldset>
</form>

