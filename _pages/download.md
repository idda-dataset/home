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
  document.getElementById("ifYes").style.display = "";
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
        <label for="car">Muu, mikä?</label> <input type="text" id="car" name="car" /><br />
    </div>
  </fieldset>
</form>

