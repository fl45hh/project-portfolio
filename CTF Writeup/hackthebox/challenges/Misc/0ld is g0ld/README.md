# 0ld is g0ld (Writeup)

Started with finding **how to view password in strings pdf**.

<img src="writeup/1.PNG" width="500px">

To view that pdf file with grab the **"/U"** for get user hash password by applied following command:

+ strings 0ld\ is\ g0ld.pdf | grep "/U"

<img src="writeup/2.PNG" width="500px">)

**John-The-Ripper** that can crack the hash value by brute forcing the wordlists

To crack the PDF file for get the **hash value** by applied following command:

+ ./pdf2john.pl /home/user/Desktop/0ld\ is\ g0ld.pdf > PDFHash.hash

<img src="writeup/3.PNG" width="500px">

To crack the hash value for get the **password** by applied following command:

+ john --wordlist=/home/user/Desktop/rockyou.txt /home/user/Desktop/PDFHash.hash

<img src="writeup/4.PNG" width="500px">

The PDF sucessfully open.

<img src="writeup/5.PNG" width="500px">

To fine the hint in the PDF file by right click and click **Read aloud**

<img src="writeup/6.PNG" width="300px">

Something fishy viewed in the PDF viewer

<img src="writeup/7.PNG" width="300px">

The **Morse Code** language formatted.

<img src="writeup/8.PNG" width="400px">

Convert the morse code to text to view the **Flag**

<img src="writeup/9.PNG" width="500px">

HTB{r1psamu31m0rs3}

**TIMEQUARTZER**
