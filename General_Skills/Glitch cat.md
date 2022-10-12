# picoCTF Glitch cat

Quite interesting, you need to have basic python knowledge or at least know how to google xD.
> Our flag printing service has started glitching!

| Commands used  | 
| ------------- | 
| [netcat](https://www.geeksforgeeks.org/netcat-basic-usage-and-overview/?ref=lbp)  | 
| python3 | 
| touch |

**You can check your python version with `python3 -V`.**

# Method of approach

1. Connect to the server with `netcat`
>  `nc saturn.picoctf.net 51109`
2. Copy the given output.
3. Close the nc connection with `ctrl+c`
4. Make a new python file with `touch flag.py`
5. Open the **flag.py** in whatever editor you want.
6. Write a print statement with the output you copied.
> print('picoCTF{gl17ch_m3_n07_' + chr(0x62) + chr(0x64) + chr(0x61) + chr(0x36) + chr(0x38) + chr(0x66) + chr(0x37) + chr(0x35) + '}'). 
8. Run the python script with `python3 flag.py`


Obviously you could solve this in other ways, but this is the hint you get from the challenge.
> We know that the glitch output is valid Python, somehow!

# picoCTF{gl17ch_m3_n07_bda68f75}



