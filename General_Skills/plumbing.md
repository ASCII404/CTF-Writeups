# picoCTF plumbing

Pretty easy, hints are more helpful than you thought.
> What's a pipe? No not that kind of pipe...

| Commands used  | 
| ------------- | 
| nc | 
| grep | 

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. 

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

# Method of approach

1. Connect to the server with `nc`
>  `nc jupiter.challenges.picoctf.org 14291`
2.  Connecting will just display a bunch of text. Change the approach.
3.  Try to `grep` the flag out of the server by using:
` nc jupiter.challenges.picoctf.org 14291 | grep pico`

Now you are getting the flag to be displayed only.

Here you can learn more about [pipes](https://www.geeksforgeeks.org/piping-in-unix-or-linux/)
# picoCTF{digital_plumb3r_ea8bfec7}
