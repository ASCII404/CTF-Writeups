# picoCTF Bases

In order to solve this problem you have to know how bases look.
> What does this bDNhcm5fdGgzX3IwcDM1 mean? I think it has something to do with bases.


| Commands used  | 
| ------------- | 
| echo | 
| base64 | 

As you can see in the commands used, I've used base64 command to find the flag as the word is base64 encoded.

# Method of approach

1. Copy the word or you can write it later.
2. Use the command `echo`.
3. Pipe it with `base64`.

The final command should look something like this:

`echo bDNhcm5fdGgzX3IwcDM1 | base64 -d`

The answer is going to be printed on your terminal or if you want to print in to a file just do:

`echo bDNhcm5fdGgzX3IwcDM1 | base64 -d > out_file.txt`

[More info about pipe](https://linuxhint.com/linux-pipe-command-examples/)

# picoCTF{l3arn_th3_r0p35}


