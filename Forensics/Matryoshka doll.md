# picoCTF Matryoshka doll

Matryoshka doll also known as stacking dolls, nesting dolls, Russian tea dolls, or Russian dolls.
> Matryoshka dolls are a set of wooden dolls of decreasing size placed one inside another. What's the final one?


| Commands used  | 
| ------------- | 
| binwalk | 
| cat | 
| exiftool |


As we know, there are going to be multiple images. Each image is going to be found inside another image.

In order to find all the images and get the flag we are going to need a tool named `binwalk`.

# Method of approach

1. Download the file with wget or by other means.
2. Check the file with `exiftool` to see if you find anything.
3. Find the `Warning : [minor] Trailer data after PNG IEND chunk`
4. Use `binwalk` on `dolls.jpg`
5. See that there is an archive which contains a directory with an image in it.
6. Extract the archive from the image with binwalk -e : `binwalk dolls.jpg -e`.
7. Go to the directory base_images and find the file `2_c.jpg`.
8. Repeat steps 6 and 7 on the new images found as many times as needed untill you find the flag:

`binwalk 2_c.jpg -e` , `binwalk 3_c.jpg -e` and so on.

I found the flag after `4_c.jpg` which was contained in a file named `flag.txt`.

9. Use cat on flag.txt to get the flag for this CTF: `cat flag.txt`.

# picoCTF{96fac089316e094d41ea046900197662}


