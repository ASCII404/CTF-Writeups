# picoCTF Information

Using adequate tools will come in handy.
> Files can always be changed in a secret way. Can you find the flag? cat.jpg


| Commands used  | 
| ------------- | 
| exiftool | 
| base64 -d | 
| echo |
| [Pipe](https://www.geeksforgeeks.org/piping-in-unix-or-linux/) |

We're using base64 -d to decode the string we found with exiftool as this is our only clue we could find about the file.

# Method of approach

1. Download the file with wget or by other means.
2. Locate the file "cat.jpg".
3. Use exiftool on cat.jpg.
4. Search for possible solutions.
5. Find a string in base64 at License: `cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9`
6. Take that string and pipe the result to echo, should look like:

`echo cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9 | base64 -d`

After decoding the string we found to be in base64 we get the flag for this CTF.

# picoCTF{the_m3tadata_1s_modified}
