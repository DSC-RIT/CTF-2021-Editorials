# Sorry

### Problem
https://dscrit-ctf-meme.netlify.app

### Flag Format
CTF{...}

### Solution
<details>
  <summary>Click to see</summary>
  
<br>

Step 1: Solve the displayed equation, the answer to which is 5.

Step 2: Now click the button 5 times. This will reveal the 1st flag (but makes you believe for a while that its the only flag).

Step 3: After about 3 seconds, another webpage shows up with "Sike that's the wrong number" meme, when reality dawns upon you (Sorry about that, hence the name of the question XD).

Step 4: Now look at the HTML file in Inspect element, there's a hidden button there. To reveal it, simply change the id given to that button to whatever you want.

Step 5: Click the revealed button, this will reveal the location of the 2nd flag (which is in Session Storage).

Step 6: Clicking the button also reveals what to do with the 1st and 2nd flags to get the final flag, which is to take the XOR of the 2 flags. That's the flag! (CTF{126777})
</details>