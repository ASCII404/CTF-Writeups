# picoCTF PW Crack 2

The second challenge comes right away with a trick which we've seen in [Glitch cat.md](https://github.com/ASCII404/CTF-Writeups/blob/main/General_Skills/Glitch%20cat.md).
> Can you crack the password to get the flag?


| Commands used  | 
| ------------- | 
| cat | 
| touch |
| python3 |

You can check your python version with `python3 -V`

# Method of approach

1. Download the files.
2. Locate the files, both must be in the same directory. 
3. Check the content of the python file with `cat`
4. Look through the file for a clue.
5. Find the following lines:

`user_pw = input("Please enter correct password for flag: ")`<br>
`if( user_pw == chr(0x33) + chr(0x39) + chr(0x63) + chr(0x65) )`

As we don't know what those hex values mean, we need to decode it first.

6. Make a new python file with `touch flag.py` or use any python file you have.
7. Write a print statement: `print(chr(0x33) + chr(0x39) + chr(0x63) + chr(0x65))`
8. Run the script with `python3 flag.py`
9. Copy the ouput.
10. Run the python file you've downloaded: `python3 level2.py`
11. Paste the ouput you copied earlier.


# picoCTF{tr45h_51ng1ng_502ec42e}


