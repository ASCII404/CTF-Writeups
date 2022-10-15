# picoCTF flag_shop.md

This challenge requires a little knowledge about C and sign rules.
> There's a flag shop selling stuff, can you buy a flag?


| Commands used  | 
| ------------- | 
| nc | 

Learn more about C data types. [Click here](https://www.tutorialspoint.com/cprogramming/c_data_types.htm)
# Method of approach

1. Download the source file for the flag shop.
2. Check the source file.

When checking the source file you can see how the balance is modified and by what is modified.

In order to change your account balance, you need to modify it by overflowing the variable.

First of all you need to look up what kind of data type your variable is.

You have a `int` which goes from `-2,147,483,648 to 2,147,483,647`

And your account balance is modified by the following code:

```
if(number_flags > 0){
      int total_cost = 0;
      total_cost = 900*number_flags;
      printf("\nThe final cost is: %d\n", total_cost);
      
      if(total_cost <= account_balance){
          account_balance = account_balance - total_cost;
          printf("\nYour current balance after transaction: %d\n\n", account_balance);
      }
```

So, if your total_cost > account_balance, then it won't enter the if condition. How can we solve that?
By making it so large that it goes negative. Why? Because it will be positive when the account balance is calculated.

For example:

`total_cost = 900*2450000` which should be equal to `-2089967296`

Now, total_cost = -2089967296, therefore your account balance is going to look like:

`account_balance = account_balance - (-2089967296); => account_balance = account_balance + 2089967296;`

4. Connect to the server with `nc`
>  `nc jupiter.challenges.picoctf.org 44566`
5. Try to buy a fake flag in order to change the account balance
6. Number of flags desired should be over 2450000 and under something like 4000000 but idk, just go for the lower limit.
7. Now after the balance is changed, buy again a flag but buy the 1337 flag.

# picoCTF{m0n3y_bag5_68d16363}
