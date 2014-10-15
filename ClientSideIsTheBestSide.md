How Nathaniel solved ClientSideIsTheBestSide
====================

Even though it has already been solved (I thought is wasn’t) I decided to do the Clients side is the best side problem and since there is no solution I thought I should explain it!

When you click on the link it provides it takes you to a webpage (porley built :P) the ask for a password. There is no way for you to guess the password but if you click inspect element then you’ll see the code behind the “website” and you see this:


<!-- standard MD5 implementation -->
<script type="text/javascript" src="md5.js"></script>
<script type="text/javascript">
  function verify() {
    checkpass = document.getElementById("pass").value;
    if (md5(checkpass) == "03318769a5ee1354f7479acc69755e7c") {
      alert("Correct!");
      document.location="./aebe515f7c62b96ad7de047c11aa3228.html";
    }
    else {
      alert("Incorrect password");
    }
  }
</script>
Now as you see it has the Verify function, so you know that that is where you’re going to check for the “Password” or a like to some other JavaScript source. Any way you can tell that it says
 if(md5(checkpass) == Blah Blah blah.) {Alert(“Correct!”)}
Now I doubt you know this but basically, MD5 is an encryption algorithm that was amazing at its time (late 1990s) but it got “Hacked” and some guy made a program that can decrypt the 32bit encryption code. 
All you have to do is copy the “blah blah blah” part and look up and md5 decipher
(Like: http://www.md5-hash.com/)
And that will give you the code “dinosaur” 
Type that in and you’ll get redirected to a webpage that says “cl13nt_s1d3_1s_w0rst_s1d3”
Then just copy and paste that to the picoCFT site and Boom you’re done!

