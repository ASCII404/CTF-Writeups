# picoCTF PW Crack 3

This challenge involves a little more python knowldege as I chose to use python in order to solve the challenge.
> Can you crack the password to get the flag? 
> 
> There are 7 potential passwords with 1 being correct. You can find these by examining the password checker script.


| Commands used  | 
| ------------- | 
| cat | 
| python3 |

You can check your python version with `python3 -V`

# Method of approach

1. Download the files
2. Locate the files 
3. Check content of the script with `cat`
4. Observe that you have those 7 passwords in the same file with the python script.
5. Write a python code that will iterate through them and try each one of them.

**The python code is going to be written in the level3.py file, just under the passwords list**

**You can use any editor you like**

The code should look something like this:

`
`


Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.


Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

# picoCTF{Lorem ipsum dolor sit amet}


