# Are you the admin?

### Problem
https://hack-into-admin-gdscrit.vercel.app/

### Flag Format
CTF{...}

### Solution
<details>
  <summary>Click to see</summary>
  
<br>


Step 1. Go to View page source

Step 2. Find this meta tag `<meta hint="Hi there 👋. This might help.. (Base 32) NB2HI4DTHIXS64TFOFRGS3ROMNXW2LY=">`

Step 3. Copy the base 32 Code and go to a Base 32 Decode (Eg - https://www.dcode.fr/base-32-encoding) and Decrypt the code. 

Step 4. This is the decoded message - https://reqbin.com/

Step 5. Upon visiting the website, you find that it is an API request tool. ( You might get an intution to check the network tab of the problem website)

Step 6. Go back to the problem website, open the network tab in developer tools

Step 7. Hit the submit button and you will see a request /auth sent to the server.

Step 8. Check the payload/ body of the request![image](https://user-images.githubusercontent.com/19583729/144702183-ac5dd886-f4ec-40f9-9bbd-51e6cc353121.png)

Step 9. Here you can find that we are sending `isAdmin` as false. So we have to send a request to the same URL with `isAdmin` as true. Here's where reqbin will help us.

Step 10. Copy the payload as a json and go to https://reqbin.com 

Step 11. Fill in the content with the JSON (making sure that `isAdmin` is set to true), set the URL , change the request to POST and click on Send. ![image](https://user-images.githubusercontent.com/19583729/144702319-82906f82-8d26-4e63-95a6-26ac908da517.png)

Step 12. In the response , you will get a JSON similar to this ```{
    "status": true,
    "message": "Login Success!!Here's your flag 😁 -> CTF{B32(IJQXU33PNNQQ====)}",
    "data": {
        "username": "admin",
        "isAdmin": true
    }
}```

Step 13. Wait, Your quest of finding the flag isn't over yet xD. There's one last step to get hold of your flag.

Step 14. As you can see , our flag seems to be this `CTF{B32(IJQXU33PNNQQ====)}` . But you will get a wrong answer if you submit it.

Step 15. The last step to this puzzle is to decode `B32(IJQXU33PNNQQ====)` , which you might have guessed, have to decode the string from Base 32.

Step 16. Go back to the same Base 32 decoder website and decode this `IJQXU33PNNQQ====`. You will be presented with a Work `Bazooka` and that's your flag🥳.

Step 17. Put the Word back into the CTF brackets by which you will get your final flag - CTF{Bazooka} 


</details>

