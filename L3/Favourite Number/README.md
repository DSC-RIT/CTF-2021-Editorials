# Favourite Number

### Problem
https://dscrit-ctf.herokuapp.com/

### Flag Format
_ _ _ E _ _ _ _

### Solution
<details>
  <summary>Click to see</summary>
  
<br>

  Step 1) Right click on input field and select ```inspect```
  
  Step 2) Look at the ```min``` and ```max``` attribute for the ```<input>``` field. You can see the number will be between 1 and 200.
  
  Step 3) Select ```Console``` in Developer Tools
  
  Step 4) Enter a guess between 1 and 200 and you'll see whether you need to go higher or lower to find the correct number. The correct guess is 133
  
  Step 5) You will get a string of numbers which you need to decode to find the final flag
  
  Step 6) Now inside Developer Tools, go to ```Application``` -> ```Local Storage```
  
  Step 7) You will find a link. Go to that link and you will find an image of an old Nokia phone with numeric keypad. This is the clue to decode the numbers.
  
  Step 8) You need to "press" the numeric keypad that many times to get the corresponding letter. For example, Pressing 4 three times on that keypad gives ``I``, therefore ```444``` -> ```I```.
  
  Step 9) Decode the entire sequence and you get the flag INVESTOR.
  
</details>
