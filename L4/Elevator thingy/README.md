# Elevator thingy

### Problem
https://gdsc-rit-question-2.herokuapp.com/

### Flag Format
CTF{...}

### Solution
<details>
  <summary>Click to see</summary>
  <br>

Step 1. Check the page source, you will find the steps written there to find the flag.<br>

Step 2. An image speaks a thousand words but we are looking for one "word" -> This tells you that the image has a word in it.<br>

Step 3. Go to https://stylesuxx.github.io/steganography/ and upload the image which is there in the website to this portal and click on "Decode". <br>

Step 4. The word is "master"<br>

Step 5. Next step is to base32 decode the word (pretty obvious) which gives you "_146"<br>

Step 6. Now, add both these strings and prefix it with "@" as instructed to give "@master_146"<br>

Step 7. The ```<marquee>``` text in the web page says "Jack Dorsey" which gives you a clue that you have to look for "@master_146" in Twitter for a clue.<br>

Step 8. In twitter you fill find a tweet by "@master_146" which says that you would have to go to "/admin" in the website to find the flag.<br>

Step 9. In http://gdsc-rit-question-2.herokuapp.com/admin, when you view the page source, you will find the flag in an html comment! (CTF{OSINT_Master})

<br>
<br>
</details>
