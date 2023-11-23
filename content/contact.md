# Contact me

<!--Bootstrap so it looks nice-->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65" crossorigin="anonymous">
<!--This is for hCaptcha-->
<script src="https://web3forms.com/client/script.js" async defer></script>
<!--This is for showing the response-->
<script type="text/javascript" src="/js/contact-us.js"></script>

<!--This is the form-->

<div class="mb-3" style="margin-top:50px"></div>
<div style="width:60%; margin:auto;">
   <form  action="https://api.web3forms.com/submit" id="contact-form" method="POST">
      <!--Don't forget to put your access key!-->
      <input type="hidden" name="access_key" value="6690e401-b723-4aa1-8394-fdde7b393841" />
      <input type="hidden" name="subject" value="new submission in contact" />
      <!--Name-->
      <div class="mb-3">
         <label for="nameInput" class="form-label">Name</label>
         <input type="text" name="name" class="form-control" id="nameInput" placeholder="Your name" required>
      </div>
      <!--Email-->
      <div class="mb-3">
         <label for="emailInput" class="form-label">Email address</label>
         <input type="email" name="email" class="form-control" id="emailInput" placeholder="name@example.com"  required>
      </div>
      <!--Message-->
      <div class="mb-3">
         <label for="messageInput" class="form-label">Message</label>
         <textarea class="form-control" name="message" id="messageInput" rows="3"  required></textarea>
      </div>
      <!--hCaptcha-->
      <div class="h-captcha" data-captcha="true"></div>
      <div class="mb-3" style="margin-top:10px">
         <button type="submit" class="btn btn-primary">Submit</button>
      </div>
   </form>
</div>
