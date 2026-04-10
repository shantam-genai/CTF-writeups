# PicoCTF 
# Challenge - Timestamped Secrets
# Category - Cryptography
# Difficulty - Medium

![alt text](<Screenshot 2026-04-10 at 12.52.09 AM.png>)

## Description : Someone encrypted a message using AES in ECB mode but they weren’t very careful with their key. Turns out it’s derived from something as simple as the current time! Can you uncover the key and decrypt the flag? Download the encrypted message: message You may also find the encryption script helpful: code

## Initial analysis: 
This challenge provides a text file and a file that contains encryption script.
From the description we get a hint of the key that is the current time.
In the text file provides a cipher text which is in hexadecimal and also the time when the encryption was done.
In the encryption script we can clearly notice the encrypt function which is taking the plain text to encrypt and the time interval as inputs.

![alt text](<Screenshot 2026-04-10 at 12.53.35 AM.png>)

![alt text](<Screenshot 2026-04-10 at 12.54.05 AM.png>)

## Approach:
So what i did, i tried to make a decryption script by analyzing the encryption script, and after running the decryption script i got the flag .

![alt text](<Screenshot 2026-04-10 at 11.12.34 PM.png>)

I got this output from running the above script.
![alt text](<Screenshot 2026-04-10 at 11.12.58 PM.png>)

Here is the flag : picoCTF{sa3S_sEc9t_081e3371}

![alt text](<Screenshot 2026-04-10 at 11.18.52 PM.png>)