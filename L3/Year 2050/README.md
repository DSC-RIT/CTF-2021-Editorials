# Year 2050

### Problem
https://dscrit-ctf-bots.netlify.app

### Flag Format
CTF{...}

### Solution
<details>
  <summary>Click to see</summary>
  <br>

Step 1: You'll see 3 binary numbers on the screen, separated by words, when the bot was speaking. Note down the numbers somewhere and join them to form just 1 binary number.<br>

Step 2: Now, look at the URL. The current route is "friend-home.html". Navigate to "my-home.html".<br>

Step 3: Click on the "Start" button to start talking to the bot.<br>

Step 4: Paste the binary number you noted down and joined earlier in the alert box. Now click Enter. This will reveal the location of the flag, which is in the window object.

Step 5: Finally, go to the console in Inspect element and type "flag" or "window.flag". This will reveal the final flag! (CTF{Humans Rule!})

<br>
</details>