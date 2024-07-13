# PRODIGY_CS_T01
 Creating a python program that can encrypt and decrypt text using the caesar cipher algorithm. Allow user to input a message and a shift value to perform encrytption and decryption. 

 Caesar Cipher is one of the most well-known and straightforward encryption methods in cryptography. The shift Cipher, Caesar's Cipher, Caesar shift, and Caesar's code, are some of its alternate names. Plain text is encrypted using this encryption method so that only the intended recipient can decipher it. Julius Caesar, who employed it in his communications, gave the approach its name.

With this encryption method, each letter in the text must be changed for a certain difference to encrypt our data. Let's imagine there is a letter "B," which becomes "C" with the left shift of 1, and "A" with the right shift of 1. Therefore, there is a difference of 1 and a text will follow the same path. Left and right shifts cannot be used simultaneously in the same text.

Algorithm of Caesar Cipher in Python
The algorithm of Caesar Cipher holds the following features :

Caesar Cipher Technique is a simple and easy method of encryption technique.
Every letter in plain text is changed to a letter that appears a certain number of positions farther down the alphabet.

To understand this algorithm in a better way let's say we want to encrypt the text "HELLO EVERYONE". Then, what we can do is change every letter in the text with a new letter that has a fixed difference. If we want to left-shift the text by 1, we must replace each letter in the previous sentence with the letter that comes after it.

Plain text: HELLO EVERYONE

Cipher text: IFMMP FWFSZPOF

As of right now, the user cannot read this text without the decryption key. The decrypt key is nothing more than the understanding of how the letters were moved during encryption. We must right shift each letter by one to decipher this.

That was Caesar Cipher's fundamental idea. The algorithm to obtain an encrypted letter will be as follows if we use a mathematical approach:

e = (a + n) mod 26

where e represents the encrypted letter's place value, a is the actual letter's position value, and n tells us the number of shifts to be done for each letter.

On the other side, we'll use the following formula to decrypt each letter:

e = (a – n) mod 26
