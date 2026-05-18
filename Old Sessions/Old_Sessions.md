# PicoCTF
# Challenge - Old Sessions
# Category - Web-Exploitation
# Difficulty - Easy

![alt text](<Screenshot 2026-05-17 at 9.08.47 PM.png>)

### Description
Proper session timeout controls are critical for securing user accounts. If a user logs in on a public or shared computer but doesn’t explicitly log out (instead simply closing the browser tab), and session expiration dates are misconfigured, the session may remain active indefinitely.This then allows an attacker using the same browser later to access the user’s account without needing credentials, exploiting the fact that sessions never expire and remain authenticated.

# Initial analysis
The challenge clearly mentions about session cookies that get stored in the websites and if not removed or cleared can be used later to unethically login without taking the permission of the real user or using the password.
![alt text](<Screenshot 2026-05-17 at 9.20.51 PM.png>)

# My Approach
So what I did is I first created a new account.
Then i saw something fishy in the comments section of the website.
![alt text](<Screenshot 2026-05-17 at 9.21.34 PM.png>)



You can clearly see that someone found something strange in '/sessions' .
So i tried it and i got the key to get the flag.
![alt text](<Screenshot 2026-05-17 at 9.18.40 PM.png>)




So here you can clearly see one thing that is the admin's session cookie is given .I went on to the session cookie and changed it with the admin's session cookie and reloaded the page.

![alt text](<Screenshot 2026-05-17 at 9.24.59 PM.png>)

![alt text](<Screenshot 2026-05-17 at 9.17.52 PM copy.png>)

So here we go ,i got the access of the admin's acount and retireved the flag.
![alt text](<Screenshot 2026-05-17 at 9.25.35 PM.png>)

Here is the flag : picoCTF{s3t_s3ss10n_3xp1rat10n5_7139c037}