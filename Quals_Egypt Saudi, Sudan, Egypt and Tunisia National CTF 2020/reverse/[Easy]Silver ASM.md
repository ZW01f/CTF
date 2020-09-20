**Silver ASM**
=======

>the flag is the parameter of the function int he following format ("FLAG{0_%X_0}" % parmter)

we got an assembly code , we can trace the code to make a simple equation to get the parmter .

>mov     eax, edx  

so eax = edx 

>add     eax, eax

eax = eax  + eax  = 2 eax 

>add     eax, edx

eax = 2 eax + eax = 3 eax 

>sal     eax, 2 

sal is **left shifts** (**multiplies**)

shift 2 bytes is equal to multiply by 4 

so eax = 4 *(3 eax ) = 12 eax 

>sub     eax, 3571200

it subtract 3571200 from eax and the code ends with zero 

so **12 eax = 3571200** 

the parmter =  0x48a80

flag : FLAG{0_48a80_0}
