CS-2024-HW4
===========


Here is a solution to 18C of the homework. Please press "RAW" to see it more clearly:

00 +1050 (Read N)
01 +1040 (Read A)
02 +2050 (Load N)
03 +3151 (Subtract 1 from N)
04 +2150 (Store N-1 in slot 90)
05 +4230 (Branch to #30 if result is 0)
06 +1041 (Read next var B)
07 +2040 (Load A)
08 +3141 (Subtract B)
09 +4120 (Branch to #20 if negative)
10 +4002 (Else branch to #2)

...

20 +2041 
21 +2140
22 +4002

(20-22 stores number in 41 in slot 40 and branches to #2)

...

30 +1140 (write 50)
31 +4300 (halt)

...

40 +0000 (var A)
41 +0000 (next var)

...

50 +0000 (N length of arguments to read)
51 +0001 (the number one)
