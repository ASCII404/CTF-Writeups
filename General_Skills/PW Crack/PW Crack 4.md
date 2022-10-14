# picoCTF PW Crack 4

This challenge is exactly as the previous one [PW Crack 3](https://github.com/ASCII404/CTF-Writeups/blob/main/General_Skills/PW%20Crack/PW%20Crack%203.md)
the only difference there is the amount of passwords.
> A for loop can help you do many things very quickly.


| Commands used  | 
| ------------- | 
| cat | 
| python3 | 

You can check your python version with `python3 -V`

# Method of approach

1. Download the files.
2. Locate the files.
3. Check content of the script with `cat`
4. Observe that you have those 100 passwords in the same file with the python script.
5. Write a python code that will iterate through them and try each one of them.

**The python code is going to be written in the level4.py file, just under the passwords list**

**You can use any editor you like**

6. Save the file after you modified it, run it to find the password.

Obviously, you could make it in a manner that would not ask you for input and it will only display your flag but I didn't care about those things, I did the first thing it came to my mind xD.

7. After you get the password, run the script again and use the password you obtained. **The password should be: eacc**

# picoCTF{fl45h_5pr1ng1ng_cf341ff1}
