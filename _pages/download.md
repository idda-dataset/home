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
        <p>Create your own scenario</p>
        <div style="width:100%; height:100%;">
         <div id="left_portion" align="center"  style="float:left; width:33%; height:10%>
        <label for="towns">Choose the town:</label><br>
            <select name="towns">
                <option value="town01">Town01</option>
                <option value="town02">Town02</option>
                <option value="town03">Town03</option>
                <option value="town04">Town04</option>
                <option value="town05">Town05</option>
                <option value="town06">Town06</option>
                <option value="town07">Town07</option>
            </select>
         </div>
         <div id="scroller" align="center" style="width:33%; height:100%; float:left>
        <label for="towns">Choose the town:</label><br>
            <select name="towns">
                <option value="town01">Town01</option>
                <option value="town02">Town02</option>
                <option value="town03">Town03</option>
                <option value="town04">Town04</option>
                <option value="town05">Town05</option>
                <option value="town06">Town06</option>
                <option value="town07">Town07</option>
            </select>
         </div>
         <div id="right_portion" align="center" style="float:right; width:33%; height:10%>
        <label for="towns">Choose the town:</label><br>
            <select name="towns">
                <option value="town01">Town01</option>
                <option value="town02">Town02</option>
                <option value="town03">Town03</option>
                <option value="town04">Town04</option>
                <option value="town05">Town05</option>
                <option value="town06">Town06</option>
                <option value="town07">Town07</option>
            </select>
         </div>
        </div>
    </div>
  </fieldset>
</form>

