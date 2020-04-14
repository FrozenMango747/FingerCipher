# Finger Cipher
## Encryption table

00-25: Lowercase Alphabet

26-51: Uppercase Alphabet

52-61: Digits 0-9

62-99: .,’”!?/\</space>[]{}()+-=_*~\`><|$&@#^%∆√</tab></enter>:;≠


## Encryption

The encryption process uses two inputs: the plaintext and the keyword / key. If the keyword is shorter than the plaintext, cycle through the characters until the string is long enough. If using a key (the U.S. Constitution, for example), trim it to the length of the plaintext. The result will be referenced later as the ‘keyphrase’.

For an example, we’ll encrypt ‘El33t’ (5 characters) with ‘Oh say can you see’ (18 characters), which we trim to ‘Oh sa’ (5 characters).

### Step 1
Convert both the plaintext and the keyphrase to numerical values using the table above. 

El33t - [30 11 55 55 19]

Oh sa - [40 07 70 18 00]

### Step 2

Add corresponding values in the matrices, but without carrying. For example, 35 + 96 = 21. 

(Subtract in mod 10 to decrypt.)

[70 18 25 63 19]
  
### Step 3

Finally, convert the ciphertext to characters:

“ qz,t”

(notice the space as the first character)
