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

<div style="word-wrap: break-word; width:auto; margin: auto; padding: 16px; box-shadow: 5px 8px 8px #CCCCCC;" >
<form action="mailto:someone@example.com" method="post" enctype="text/plain" style="background: none;">
  <fieldset>
    <legend><b>Compile this form to request the dataset or a single split</b></legend>
    <p><br><br><br></p>
    <label for="fname">Name:</label><br>
    <input type="text" id="fname" style="word-wrap: break-word; word-break: break-all; border: none; border-bottom: 0.01em solid gray;" required><br>
    <label for="lname">Surname:</label><br>
    <input type="text" id="lname" style="word-wrap: break-word; word-break: break-all; border: none; border-bottom: 0.01em solid gray;" required><br>
    <label for="email">Email:</label><br>
    <input type="email" id="email" style="word-wrap: break-word; word-break: break-all; border: none; border-bottom: 0.01em solid gray;" required><br>
    <label for="company">Organization:</label><br>
    <input type="text" id="company" style="word-wrap: break-word; word-break: break-all; border: none; border-bottom: 0.01em solid gray;"><br>
    <label for="reason">Reason for use of dataset:</label><br>
    <input type="text" id="reason" style="word-wrap: break-word; word-break: break-all; border: none; border-bottom: 0.01em solid gray; height: 150px;" required><br>
    Do you want the whole dataset?<br>
    <select id="mySelect" onchange="myFunction();" required>
        <option value=""></option>
        <option value="yes">Yes</option>
        <option value="no">No</option>
    </select>
    <p id="demo"></p>
    <div id="ifYes" style="display: none;">
        <p>Create your own scenario</p>
        <div style="width:100%; height:100%;">
            <label for="towns">Town:</label>
            <select name="towns" required>
                <option value=""></option>
                <option value="town01">Town 01</option>
                <option value="town02">Town 02</option>
                <option value="town03">Town 03</option>
                <option value="town04">Town 04</option>
                <option value="town05">Town 05</option>
                <option value="town06">Town 06</option>
                <option value="town07">Town 07</option>
            </select>
            <br>
            <label for="weather">Weather and illumination condition:</label>
            <select name="weather" required>
                <option value=""></option>
                <option value="weather1">Clear Noon</option>
                <option value="weather2">Clear Sunset</option>
                <option value="weather3">Hard Rain Noon</option>
            </select>
            <br>
            <label for="viewpoint">Vehicle Viewpoint:</label>
            <select name="viewpoint" required>
                <option value=""></option>
                <option value="audi">Audi TT</option>
                <option value="mustang">Ford Mustang</option>
                <option value="jeep">Jeep Wrangler Rubicon</option>
                <option value="volkswagen">Volkswagen T2</option>
                <option value="bus">Bus</option>
            </select>
            <br>
        </div>
    </div>
    <p><br><br></p>
    <input type="submit" value="Request" class="btn--disabled"/>
  </fieldset>
</form>
</div>
<br>
<br>
<br>

Dataset download will be available soon. You can now download a preview of IDDA [here](www.prova.com)
{: .notice--warning}