# Missing Files

### Problem
https://load-network.herokuapp.com/

### Flag Format
; _ _ H _ _ _ !

### Solution
<details>
  <summary>Click to see</summary>
  <br>

Step 1) Inspect the page and click on 'Network'. You can observe that allow.js and mail.js are missing. <br>

Step 2) Console says report missing files in missing_section. -> So you have to report missing files in /missing_section route.<br>

Step 3) Enter allow.js in /missing_section.<br>

Step 4) If you inspect the html you find that multiple input tags are hidden and it contains links as its values.<br>

Step 5) If you view style3.css in source.It instructs you to use #hify to decode -> it implies to use the link which has the id hify.<br>

Step 6) Visit the link and submit the background image to decode the hidden value -> the hidden key is @DSC-Stegano<br>

Step 7) submit the hidden key.You get the second half of the flag as ~Ct!<br>

Step 8) Now visit /missing_section and report mail.js<br>

Step 9) If you visit style2.css you can see that key is CAPS_LOCK( --. .-. . .- -) in .box::before.<br>

Step 10) On decoding the morse code. You get GREAT.<br>

Step 11) Submit the key.<br>

Step 12) You get the first half of the flag as ;mIH.<br>

Step 13) Combine the first half and second half.<br>

Step 14) The flag is ;mIH~Ct!<br>

<br>
</details>