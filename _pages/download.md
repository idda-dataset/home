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
{%
function yesnoCheck(that) {
    if (that.value == "no") {
        document.getElementById("ifYes").style.display = "block";
    } else {
        document.getElementById("ifYes").style.display = "none";
    }
}
%}

<form action="mailto:someone@example.com" method="post" enctype="text/plain">
  <fieldset>
    <legend>Compile this form to request the dataset or a split</legend>
    <label for="name">Name and Surname:</label><br>
    <input type="text" id="name"><br>
    <label for="email">Email:</label><br>
    <input type="email" id="email"><br>
    Do you want the whole dataset?<br>
    <select onchange="yesnoCheck(this);">
        <option value=""></option>
        <option value="yes">Yes</option>
        <option value="no">No</option>
    </select>
    <div id="ifYes" style="display: none;">
        <label for="car">Muu, mikä?</label> <input type="text" id="car" name="car" /><br />
    </div>
  </fieldset>
</form>

