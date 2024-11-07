# PicoCTF-writeup
(Work in progress)
## Easy1
### Question
![Screenshot 2024-11-07 194504](https://github.com/user-attachments/assets/9b654f3f-dd9b-4d16-90be-8f5de3b7ae0d)
### Given Table
![Screenshot 2024-11-07 195220](https://github.com/user-attachments/assets/4e902790-7b44-4d68-a11c-24837c430b0f)
### Solution
Not so obvious at first, but the table gives subtle hints on how to use it. After much trial and error that took time, I found out that the algorithm I was supposed to follow to find the key was:
1. Go to the row of the letter in the key
2. Traverse to the column of the corresponding letter of the ciphertext
3. Look at the columnm header of the letter, that is the letter of the flag
4. Repeat steps 1-3 until you run out of letters in key
### Flag
The flag hence found is CRYPTOISFUN, which can be input as picoCTF{CRYPTOISFUN}

## Vigenere
### Question
![Screenshot 2024-11-07 194625](https://github.com/user-attachments/assets/577ef36b-7639-4417-ba61-580f7d412ce9)
### Given Message
rgnoDVD{O0NU_WQ3_G1G3O3T3_A1AH3S_cc82272b}
### Hint
A link to Wikipedia page of Vigenère cipher
### Solution
It was pretty straightforward once I knew this was Vigenère cipher, Just go to a decode tool such as [dcode](https://www.dcode.fr/en), search for Vigenere Cipher decoder tool, enter the key and press decrypt, and get the flag.
![Screenshot 2024-11-07 202403](https://github.com/user-attachments/assets/8997e1b1-d68b-4546-9709-a41aef440801)
### Flag
picoCTF{D0NT_US3_V1G3N3R3_C1PH3R_ae82272q}
