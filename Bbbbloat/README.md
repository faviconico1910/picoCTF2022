Bbbbloat

---------------------------------------------------------------------
AUTHOR: LT 'SYREAL' JONES

Description
Can you get the flag?

Reverse engineer this binary.
![image](https://github.com/faviconico1910/picoCTF2022/assets/165459765/72c1961d-ac5b-4f49-abca-cd8663daf065)

- Check with terminal, it is ELF 64-bit pie executable

![image](https://github.com/faviconico1910/picoCTF2022/assets/165459765/679774b3-f55c-4243-b424-dadafa0cea2e)

- Then, open it with IDA 64 bit free :>, select main, press Tab to toggle pseudocode and disassembly views.


![image](https://github.com/faviconico1910/picoCTF2022/assets/165459765/6f8409f4-a3e9-4e4d-8bde-ef488ff1bdc5)

- Now, we can see maybe if we pass the integer 549255, the program will display the flag. Let's try it

![image](https://github.com/faviconico1910/picoCTF2022/assets/165459765/b0061d9a-a59f-4955-8bb2-3b648b31d8e1)

---------------------------------------------
Flag: picoCTF{cu7_7h3_bl047_44f74a60}









