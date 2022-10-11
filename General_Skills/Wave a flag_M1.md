# picoCTF Wave a flag

I got 2 solutions for this challenge, this writeup is the first solution.

Both solutions work, pick whatever you feel like using.

Second solution:[Wave a flag_M2.md](https://pages.github.com/)
> Python scripts are invoked kind of like programs in the Terminal...

| Commands used  | 
| ------------- | 
| python3 / python | 
| wget | 
| cat | 

Depdends on what version of python you have installed on your machine.

Check it in the terminal with `python --version` or `python3 --version`
# Method of approach

1. Download the file with wget or by other means:
>  `wget https://mercury.picoctf.net/static/0bf545252b5120845e3b568b9ad0277e/ende.py`
2. Download the remaining files and locate all of them.
3. Use `python3 ende.py` to run the script.
You're going to see the following line:
> Usage: ende.py (-e/-d) [file]

We assume that `-e` stands for encode and `-d` for decode.

By checking the **pw.txt** file we can see something which seems to be **encoded in base64**.
> 6008014f6008014f6008014f6008014f

4. Run `python3 -d flag.text.en`


A message is going to be prompted such as: 
>Please enter the password:

In which you are going to put that **64base encoded** text we saw in the **pw.txt**
# picoCTF{4p0110_1n_7h3_h0us3_6008014f}


