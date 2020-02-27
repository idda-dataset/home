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
    <label for="fname">Name:</label><br>
    <input type="text" id="fname" required><br>
    <label for="lname">Surname:</label><br>
    <input type="text" id="lname" required><br>
    <label for="email">Email:</label><br>
    <input type="email" id="email" required><br>
    <label for="company">Academy/Institution/Company name:</label><br>
    <input type="text" id="company"><br>
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
            <div id="left_portion" align="center"  style="float:left; width:20%; height:100%">
                <label for="towns">Select the town:</label><br>
                <select name="towns">
                    <option value=""></option>
                    <option value="town01">Town01</option>
                    <option value="town02">Town02</option>
                    <option value="town03">Town03</option>
                    <option value="town04">Town04</option>
                    <option value="town05">Town05</option>
                    <option value="town06">Town06</option>
                    <option value="town07">Town07</option>
                </select>
            </div>
            <div id="scroller" align="center" style="width:60%; height:100%; float:left">
                <label for="weather">Select the weather condition:</label><br>
                <select name="weather">
                    <option value=""></option>
                    <option value="weather1">Clear Noon</option>
                    <option value="weather2">Clear Sunset</option>
                    <option value="weather3">Hard Rain Noon</option>
                </select>
            </div>
            <div id="right_portion" align="center" style="float:right; height:100%">
            <label for="viewpoint">Select the viewpoint:</label><br>
                <select name="viewpoint">
                    <option value=""></option>
                    <option value="audi">Audi TT</option>
                    <option value="mustang">Ford Mustang</option>
                    <option value="jeep">Jeep Wrangler Rubicon</option>
                    <option value="volkswagen">Volkswagen T2</option>
                    <option value="bus">Bus</option>
                </select>
            </div>
        </div>
    </div>
    <input type="submit" value="Request" class="btn--disabled">
  </fieldset>
</form>

<br>
<br>
<br>
Dataset download will be available soon. You can now download a preview of IDDA following the [link](www.prova.com)
{: .notice--warning}