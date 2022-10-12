# picoCTF strings it

This challenge is quite simple if you know the `strings` command.
> Can you find the flag in file without running it?

There might be a lot of approaches but you don't need anything complex for it. Keep it simple.


| Commands used  | 
| ------------- | 
| strings | 
| grep | 

If you want to know more about `strings` just do `strings -h` in the terminal and play with it.

# Method of approach

1. Download the file.
2. Locate the file
3. Use `strings` and **pipe** it with `grep`

The final command should look like: `strings strings | grep pico` 

The reason why we are using **pico** as a keyword is that we know that there's a flag somewhere and we also know the format of the flag. 

You can use any **keyword** related to the flag in order to achieve it.

# picoCTF{5tRIng5_1T_d66c7bb7}


