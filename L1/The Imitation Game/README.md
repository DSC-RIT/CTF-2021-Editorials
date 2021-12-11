# The Imitation Game

### Problem
https://ctf-l2q5.herokuapp.com/

### Flag Format
B _ _ _ _ _ A

### Solution
<details>
  <summary>Click to see</summary>
  
<br>

Step 1: Right click to 'inspect' </br>

Step 2: Observe how there are 3 divs (boxes) but only 2 divs (boxes) are displayed</br> 

Step 3: Move over to the style tag and remove the display property with the value 'none' for box b3</br> 

Step 4: use pigpen cipher to decrypt the text contained within the third box to get the flag (bazinga)

</details>