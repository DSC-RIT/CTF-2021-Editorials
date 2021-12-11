# Servers and Flags

### Problem
https://trusting-volhard-cf852d.netlify.app/#/

### Flag Format
K _ _ _ _ _ _ _ _ 4

### Solution
<details>
  <summary>Click to see</summary>
  <br>
  
Step 1. Clues/info to note in the question: 'Node' and 'header'. So, we must supply a suitable **header** and it's value, which should be added to the **nodeJS** server, in order to "fix" it and hence obtain our flag.<br>

Step 2. First, let's try adding some random values to both fields and click on 'get flag'. As expected, it doesn't work. But why? Head over to the 'network' tab under inspect.<br>

Step 3. It informs us that a CORS error is occuring [(why?)](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) ! So clearly, we need to add a header to fix it.<br>

Step 4. Upon browsing for ways to fix a CORS error, we find that ```res.header("Access-Control-Allow-Origin", "*");``` is a common fix, without using any external npm packages. <br>

Step 5. So, enter in "Access-Control-Allow-Origin" and "*" in the respective fields and voila, flag appears. (KEYiodj434)<br>
<br>

**NOTE**: For those of you wondering why you shouldn't make a direct call to the API end-point through your browser- we've coded it in such a way that the flag must be received through the app only (the app performs a decription to give you the flag in the right format)! So, correctly identifying and fixing the CORS error is a necessary step, which can't be bypassed.

<br>
</details>

