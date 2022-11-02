# Encryption_Decryption_using_Mips
This project is an I/O console to encrypt and decrypt text using a simple ciphers. Specifically you will encrypt and decrypt text with a Vigenere cipher, which is a simple extension of the ` well know Caesar cipher, where letters are shifted by a given number

# Project Discription

Specifically you will encrypt and decrypt text with a Vigenere cipher, which is a simple extension of the `
well know Caesar cipher, where letters are shifted by a given number. For instance a shift of 3 would
change an A to D. At the end of the alphabet, we wrap back to the beginning, so a shift of 3 also changes
a Z to C.

We will assume that all text is ASCII, and we will work only with capital letters. The key will also be
written using letters where A corresponds to a shift of 0, B to 1, C to 2, and so on. Decryption is done by
simply shifting instead by a negative amount.

In a Vigenere cipher, to use a key with multiple letters, `
we repeat the key over and over again. Where the plain
text contains spaces and punctuation, we will leave the text
unchanged, and skip to the next letter in the key and the
next letter in the text. For instance ”LET’S GO TO THE CAT
MUSEUM!” with key ”AB” will becomes ”LFT’S GP UO TIE
CBT MVSFUN!”, that is, letters in even positions starting at
position zero are not shifted, while letters in odd positions
are shifted by 1.

There are many interesting ways to try to break Vigenere `
ciphers, but among the most simple is to look at letter
frequencies. In this assignment, you will be required to
compute the frequencies of letters to try to identify the key,
but this will not be an entirely automatic process. For a given
guess, you will need to also specify an assumed length of the key and what letter you believe to be most
probable. While the letter E is most common in large blocks of English text, other letters are also very
common

# Code discription
The provided code implements a simple command menu to let you read a text file into a buffer, print
the text in the buffer, encrypt the buffer, decrypt the buffer, write the buffer to a file, guess an encryption
key, and quit.
# EncryptBufferImplement the EncryptBuffer procedure.

This procedure takes two arguments. The first is a null terminated
ASCII string to encrypt (i.e., the text buffer), while the second is a null terminated ASCII string for the
key. We can assume that the letters in the buffer are all uppercase, and likewise, that the key is specified
with all uppercase letters. We should leave any non-letters unchanged (e.g., punctuation and white
spaces).
# DecryptBuffer
Implement the DecryptBuffer procedure. This procedure takes two arguments. The first is a null terminated
ASCII string to decrypt (i.e., the text buffer), while the second is a null terminated ASCII string for the
key. We can assume that the letters in the buffer are all uppercase, and likewise, that the key is specified
with all uppercase letters. 
# GuessKey
Implement the GuessKey procedure, The procedure takes 4 arguments: the size of the key to guess, the null
terminated text buffer, a block of memory in which to write the guessed key (i.e., you are returning the
guessed key to the caller in this memory), and finally the last parameter is the letter which we can assume
to be most common in the cypher text.
