# unpackme

-----
AUTHOR: LT 'SYREAL' JONES

Description

Can you get the flag?

Reverse engineer this [binary](https://artifacts.picoctf.net/c/205/unpackme-upx)

  ![image](https://github.com/faviconico1910/picoCTF2022/assets/165459765/c193c332-456e-4252-9fd2-33f6cf1bdfa4)

-	Try run it, we know that this challenge requires a number
  ![image](https://github.com/faviconico1910/picoCTF2022/assets/165459765/c12486b0-5494-4e5f-9d56-2bcd0267fc70)


-	It hints us about **UPX**, and the title is unpackme, so we guess this binary file is packed by **UPX** -> install it in **Kali Linux**

  ![image](https://github.com/faviconico1910/picoCTF2022/assets/165459765/6952caa5-9028-461f-8f63-c8eda74cf247)

-	Now, try decompress it

  ![image](https://github.com/faviconico1910/picoCTF2022/assets/165459765/a10ef942-b715-4474-8823-edf4b0df2253)

-	We can observe that the file size increased from 379188 to 1006445 with ratio 37,68%
-	Now, disassemble it, we have to look at cmp instruction which compare eax registers from scanf with the value 0xb83cb

  ![image](https://github.com/faviconico1910/picoCTF2022/assets/165459765/dc51228f-1774-4390-a139-59e8a14e57da)

-	Convert 0xb83cb into decimal

  ![image](https://github.com/faviconico1910/picoCTF2022/assets/165459765/dac85bd4-bd17-4715-a7f7-9e12629f3862)

  -	Run and pass this value

  ![image](https://github.com/faviconico1910/picoCTF2022/assets/165459765/536fb2b7-9060-432e-9c43-8449910d274d)

  -------
  Flag: picoCTF{up><_m3_f7w_5769b54e}








  

