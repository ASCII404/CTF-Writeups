# picoCTF PW Crack 3

This challenge involves again little python knowledge. But this only because I chose to use python in order to solve the challenge.
> Can you crack the password to get the flag? 
> 
> There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.


| Commands used  | 
| ------------- | 
| cat | 
| python3 |

You can check your python version with `python3 -V`

# Method of approach

1. Download the files.
2. Locate the files.
3. Check content of the script with `cat`
4. Observe that you have those 7 passwords in the same file with the python script.
5. Write a python code that will iterate through them and try each one of them.
6. Save the file after you modified it, run it to find the password.

**The python code is going to be written in the level3.py file, just under the passwords list**

**You can use any editor you like**

The code should look something like this:

![Python script modified](https://github.com/ASCII404/CTF-Writeups/blob/main/General_Skills/PW%20Crack/pwcrack3.png)

Obviously, you could make it in a manner that would not ask you for input and it will display your flag but I didn't care about those things, I just wanted the flag.

7. After you get the password, run the script again and use the password you obtained. **The password should be: 4b17**

# picoCTF{m45h_fl1ng1ng_2b072a90}


