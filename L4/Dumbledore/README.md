# Dumbledore

### Problem
https://albus-dumbledore.herokuapp.com/

### Flag Format
1 _ _ _ _ _ _

### Solution
<details>
  <summary>Click to see</summary>
  <br>

Step 1) The encrypted key is 100000010101<br>

Step 2) Storage is highlighted. If you visit session storage, you will find the instructions to find flag.<br>

Step 3) If you find data.js in source.You can find multiple instance of AUrelius DUmbledore. Compare the cases to find the correct one. <br>

Step 4) The correct one tells us to convert packed bcd to decimal. On converting you get the decrypted value as 815. <br>

Step 5) The key value is /potter. Visit /potter route to find the second key.<br>

Step 6) If you inspect the /potter. you can find a hidden p tag.<br>

Step 7) The p tag hints us towards Cookies.<br>

Step 8) The second key 524 is present in cookies.<br>

Step 9) If you find array.js in source.You can find multiple instance of Operations. Compare the cases to find the correct one. <br>

Step 10) The Operation is gate. Try different gate operation.<br>

Step 11) The correct Operation is nand gate.<br>

Step 12) Perform the operation present in session storage to get flag 1FE995B.    <br>

 
 
<br>
</details>
