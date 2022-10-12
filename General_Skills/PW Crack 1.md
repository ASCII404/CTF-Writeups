# picoCTF PW Crack 1

This is the first challenge from a total of 5 same others. 

Think about them as levels, even though you don't need to complet them in order,
it helps to get through them with little steps.
> Can you crack the password to get the flag?


| Commands used  | 
| ------------- | 
| cat | 
| python3 |  

You can check your python version with `python3 -V`

# Method of approach

1. Download the files.
2. Locate the files, both must be in the same directory. 
3. Check the content of the python file with `cat`
4. Look through the file for a clue.
5. Find the statement:

`user_pw = input("Please enter correct password for flag: ")`<br>
`if( user_pw == "1e1a")`

As you can see, the required input is stored in `user_pw` which it is verified in the `if(user_pw == 1e1a)`

Then we can assume that the required password for the flag is **1e1a**.

6.Run the script with `python3 level1.py`
7. Use the password found in the script.

# picoCTF{545h_r1ng1ng_fa343060}
