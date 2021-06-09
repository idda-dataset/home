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
$(document).ready(function() {
    $('.js-example-basic-single').select2();
});
</script>

<div style="word-wrap: break-word; width:auto; margin: auto; padding: 16px; box-shadow: 5px 5px 5px 5px #CCCCCC; background-color:White;" >

<form accept-charset="UTF-8" style="background-color:White;" action="https://getform.io/f/da0906d1-21bc-42cc-ba85-6dc77904a443" method="POST" enctype="multipart/form-data" target="_blank">
  <fieldset>
    <legend><b>Compile this form to request one or more splittings of IDDA</b></legend>
    <p><br><br><br></p>
    <label for="fname">Name*:</label><br>
    <input type="text" id="fname" name="name" style="border: none; border-bottom: 0.01em solid gray;" required><br>
    <label for="lname">Surname*:</label><br>
    <input type="text" id="lname" name="surname" style="border: none; border-bottom: 0.01em solid gray;" required><br>
    <label for="email">Email*:</label><br>
    <input type="email" id="email" name="email" style="border: none; border-bottom: 0.01em solid gray;" required><br>
    <label for="company">Organization:</label><br>
    <input type="text" id="company" name="organization" style="border: none; border-bottom: 0.01em solid gray;"><br>
    <label for="reason">Reason for use of dataset*:</label><br>
    <textarea id="reason" name="reason" style="border: none; border-bottom: 0.01em solid #808080;" rows="5" required></textarea><br>
    <label for="choice">Choose the subset/s you want to download:</label><br>
    <select class="js-example-basic-multiple" name="splitttings" multiple="multiple">
    <option name="best" value="Splitting Best">Splitting Best</option>
    <option name="worst" value="Splitting Worst">Splitting Worst</option>
    <option name="t01csa" value="T01 CS A">T01 CS A</option>
    <option name="t01csj" value="T01 CS J">T01 CS J</option>
    <option name="t01hrna" value="T01 HRN A">T01 HRN A</option>
    <option name="t01hrnj" value="T01 HRN J">T01 HRN J</option>
    <option name="t07hrna" value="T07 HRN A">T07 HRN A</option>
    </select>
    <input type="submit" value="Request" class="btn--success"/>
  </fieldset>
</form>
</div>
<br>
<br>
<br>

*Required field<br>
Dataset download will be available next week. You will receive download link by email. More splittings will be added soon. 
{: .notice--warning}