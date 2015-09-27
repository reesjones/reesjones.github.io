---
title: Contact Me
layout: page
---

<form class="form-horizontal"
	action="//formspree.io/mitchrj196@gmail.com"
	method="POST">

<fieldset>

<legend>Send me something here</legend>

<div class="form-group">
  <label class="col-md-4 control-label" for="email">Your email</label>  
  <div class="col-md-4">
  <input id="email" 
		name="email" 
		type="text" 
		style="width: 50%;"
		placeholder="foo@bar.com" 
		class="form-control input-md">
    
  </div>
</div>

<div class="form-group">
  <label class="col-md-4 control-label" for="message">Your message</label>
  <div class="col-md-4">                     
    <textarea class="form-control" id="message" name="message"
		style="width: 50%; height: 200px;"></textarea>
  </div>
</div>

<div class="form-group">
  <label class="col-md-4 control-label" for="send"></label>
  <div class="col-md-4">
    <button id="send" name="send" class="btn btn-primary"
		style="background-color: #848482;">Send</button>
  </div>
</div>

<!-- Formspree hidden fields -->
<input type="hidden" name="_subject" value="Message from reesjones.github.io" />
<input type="text" name="_gotcha" style="display:none" />

</fieldset>
</form>

