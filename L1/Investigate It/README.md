# Investigate it

### Problem
https://gdsc-ctf-2021.herokuapp.com/

### Flag Format
Y_ _  _ _ _ _ _ _ D  _ T

### Solution
<details>
  <summary>Click to see</summary>
  
<br>
Step 1) Right click to "Inspect" 

Step 2) Under ```<head>``` go to ```<style>```

Step 3) Change color in p.key to any color other than cyan and then hover over the button "Try this for the key", say black.

-> The similar color of the text and background makes the flag invisible; changing it to any other color will make it visible on the screen.
  
Alternate solution: In the ``` <script> ``` tag, key can be found in key_out() funtion.

Key: YOU CRACKED IT
</details>