# Challenges

## Mod 26 
To solve this challenge, we simply had to decode the ROT13 (Caesar Cipher) and get the flag. 

### Solution 
To solve this challenge, I simply copied the string given to us in the challenge description and copied it onto cyberchef.io to get the answer. I used ROT13 as mentioned in the question. 

### Flag

`picoCTF{next_time_I'll_try_2_rounds_of_rot13_ZNMldSDw}` 

### Notes
Simple practice of using ROT13, logical rotation to 13th alphabet from start position. 

### References
- https://play.picoctf.org/practice/challenge/144?page=1&search=mod%2026
- https://cyberchef.io/
-----------------------------------------------------------------------------------------------------------------------------------
## 13 
This challenge also needed us to use ROT13 to get the flag. 

### Solution 
I simply used cyberchef.io again on the line given to us in the challenge statement to get the flag. 

### Flag
`picoCTF{not_too_bad_of_a_problem}`

### Notes
This was again pretty simple challenge

### References
- https://play.picoctf.org/practice/challenge/62?page=1&search=13
- https://cyberchef.io/
-----------------------------------------------------------------------------------------------------------------------------------
## Interncdec
To solve this challenge, we had to use base64 to solve it.

### Solution 
To solve this challenge, I followed the steps as given below: 
- I first downloaded the file from the challenge, then used the `cat` command to get the data out from the file. Seeing that the data ended in `==`, I realized that it was base64 endcoded. Putting this again in cyberchef.io, I got a python type string, i.e., it was of the type `b'....'`.
- The data inside the single quotes was further base64 encoded, so selecting only that data, I got data in some random format as shown:

```bash
wpjvJAM{jhlzhy_k3jy9wa3k_i204hkj6}
```
- Now seeing that this data already had curly braces, I got the idea to use ROT13 again, except changing the ROT value to find the flag. The correct roation value turned out to be 19 which I found by trial and error.

### Flag
`picoCTF{caesar_d3cr9pt3d_b204adc6}` 

### Notes
This turned out to be a pretty fun challenge, with good revision for base64 and Caesar Cipher. 

### References
- https://play.picoctf.org/practice/challenge/418?page=1&search=inter
- https://cyberchef.io/
------------------------------------------------------------------------------------------------------------------------------------
