# picoCTF Wave a flag
>Can you invoke help flags for a tool or binary?


| Commands used  | 
| ------------- | 
| cat | 
| grep|

# Method of approach

1. Download the file with wget or by other means:
>  `wget https://mercury.picoctf.net/static/b28b6021d6040b086c2226ebeb913bc2/warm`

2. Locate the file.
3. Use `cat` in order to output the content and `grep` to get the flag.
4. Those commands combined are going to look like: `cat warm | grep -a pico`

Output is going to look something like:
> ]��f.�]�@f.�H�=� H��t    H�5�	 UH)�H��H��H��H��?H�H��tH��	 H��t
                                                                     ]��f�]�@f.��=y	 u/H�=W	 UH��t
����H����Q       ]����fDUH��]�f���UH��H���}�H�u��}�uH�=������KH�E�H�H�H�5�H��������uH�=��i����H�E�H�H�H��H�=:��X������DAWAVI��AUATL�%F UH�-F SA��I��L)�H�H�������H��t 1��L��L��D��A��H��H9�u�H�[]A\A]A^A_Ðf.���H�H��Hello user! Pass me a -h to learn what I can do!-hOh, help? I actually don't do much, but I do have this flag here: **pico**CTF{b1scu1ts_4nd_gr4vy_d6969390}I don't know what '%s' means! I do know what -h means though

# picoCTF{b1scu1ts_4nd_gr4vy_d6969390}


