# Concepts 

## Base64 Encode
Base64 is an encoding scheme used to represent binary data (like images or files) in an ASCII string format by translating it into a radix-64 representation using 64 printable characters. This is necessary for safely transmitting binary information over systems like email that were originally designed only to handle 7-bit ASCII text, though it results in the encoded data being approximately one-third larger than the original. Dead give away for base64 encoded data is that it usually ends with `==`.

## Caesar Cipher
The Caesar cipher is one of the simplest and oldest encryption techniques (a type of single alphabet substitution cipher) where each letter in the plaintext is shifted a fixed number of positions down or up the alphabet, with the shift value acting as the secret key. This shift wsa historically only 3 alphabets, but can be any number of characters.

## Vigenere Cipher
The Vigenère cipher is a method of encrypting alphabetic text using a series of interwoven Caesar ciphers, which makes it a type of polyalphabetic substitution cipher. It uses a keyword to determine the shift for each letter of the plaintext; the keyword is repeated to match the length of the message. For example, if the keyword is "KEY" and the message is "ATTACK", the key applied would be "KEYKEY". Each letter of the message is shifted by an amount corresponding to the position of the key letter (A=0, B=1, etc.) in the alphabet. This key-dependent, variable shifting is its strength, as it ensures that the same plaintext letter can be encrypted to different ciphertext letters throughout the message, thereby largely defeating basic frequency analysis, a simple code-breaking technique that works easily on the simpler Caesar cipher.
