# picoCTF Wave a flag

I got 2 solutions for this challenge, this writeup is the first solution.

Both solutions work, pick whatever you feel like using.

Second solution: [Wave a flag_M2.md](https://github.com/ASCII404/CTF-Writeups/blob/main/General_Skills/Wave%20a%20flag_M2.md)

>Can you invoke help flags for a tool or binary?


| Commands used  | 
| ------------- | 
| wget | 
| chmod |

# Method of approach

1. Download the file with wget or by other means:
>  `wget https://mercury.picoctf.net/static/b28b6021d6040b086c2226ebeb913bc2/warm`
>  
2. Locate the file.
3. Use `chmod +x warm` in order to be able to execute the file.
4. Run the file `./warm`


# picoCTF{b1scu1ts_4nd_gr4vy_d6969390}


