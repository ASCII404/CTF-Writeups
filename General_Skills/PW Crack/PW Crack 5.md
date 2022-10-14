# picoCTF PW Crack 5

The final challenge in this series. Not that hard, the same as PW Crack 3 and PW Crack 4 just a little extra step.
> Here's a dictionary with all possible passwords based on the password conventions we've seen so far.


| Commands used  | 
| ------------- | 
| cat | 
| python3 | 

You can check your python version with `python3 -V`

# Method of approach

1. Download the files.
2. Locate the files.
3. Check content of the script with `cat`
4. Observe that you don't have a list with all the passwords.
5. Be sure to have all files in the same directory.
6. Write a python code that will iterate through the **dictionary.txt** and try each one of the passwords.

 **The python code is going to be written in the level5.py file, just that we are reading from another file**

**You can use any editor you like**

7. Save the file after you modified it, run it to find the flag.

The code should look something like this:

![Python script modified](https://github.com/ASCII404/CTF-Writeups/blob/main/General_Skills/PW%20Crack/pwcrack5.png)

# picoCTF{m45h_fl1ng1ng_2b072a90}


