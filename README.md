# PicoCTF-writeup
(Work in progress)
## Easy1
### Question
![Screenshot 2024-11-07 194504](https://github.com/user-attachments/assets/9b654f3f-dd9b-4d16-90be-8f5de3b7ae0d)
### Given Table
![Screenshot 2024-11-07 195220](https://github.com/user-attachments/assets/4e902790-7b44-4d68-a11c-24837c430b0f)
### Solution
Not so obvious at first, but the table gives subtle hints on how to use it. After much trial and error, I found out that the algorithm I was supposed to follow to find the key was:
1. Go to the row of the letter in the key
2. Traverse to the column of the corresponding letter of the ciphertext
3. Look at the columnm header of the letter, that is the letter of the flag
4. repeat steps until you run out of letters in key

### Flag
The flag hence found is CRYPTOISFUN, which can be input as picoCTF{CRYPTOISFUN}
