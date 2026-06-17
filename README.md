# Cryptographic Fundamentals (Caesar Cipher)
In the world of cybersecurity, encryption plays a crucial role in protecting sensitive information. One of the simplest and oldest forms of encryption is the Caesar Cipher, named after Julius Caesar, who reportedly used this method to communicate secretly with his generals, the Caesar Cipher provides an excellent starting point for understanding basic cryptographic concepts.

In this tutorial, we will walk through how to implement a Caesar Cipher in Python, allowing you to both encrypt and decrypt messages.

## Content
- []()

## What is the Caesar Cipher?
The **Caesar Cipher** is a substitution cipher which works by shifting each letter of a message (plaintext) by a fixed number of positions in the alphabet. This fixed number is known as the **"key"** or **"shift"**.

Here's how it works:

1. Choose a key (let's say 3).
2. For each letter in your message:
   - Shift it forward in the alphabet by the number of positions specified by the key.
   - If you reach the end of the alphabet, wrap around to the beginning.
3. Non-alphabetic characters (spaces, punctuation) remain unchanged.

For example, with a shift of 3:
- 'A' becomes 'D'
- 'B' becomes 'E'
- 'Y' becomes 'B' (wrapping around)
- 'Z' becomes 'C' (wrapping around)
  
So, the message **"HELLO WORLD"** with a shift of 3 would become **"KHOOR ZRUOG"**.
- During encryption, each letter in the message is shifted forward in the alphabet by the key value.
- During decryption, each letter in the encrypted message is shifted backward in the alphabet by the key value.
- The shift wraps around the alphabet, meaning if we go past Z, we loop back to A.
