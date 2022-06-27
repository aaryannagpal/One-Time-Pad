# One-Time-Pad

In cryptography, the one-time pad is an encryption technique that cannot be cracked, but requires the use of a single-use pre-shared key that is not smaller than the message being sent. 

In this technique, a plaintext is paired with a random secret key (also referred to as a one-time pad). Then, each bit or character of the plaintext is encrypted by combining it with the corresponding bit or character from the pad using **XOR** operation.

In my version of the encryption, every character of the plaintext is first converted into binary. Then, a random binary key is created for each character, of the same length for the XOR operation to work smoothly. After the keys are randomly generated for each character, the XOR operation between the binary plaintext character and its corresponding key takes place, resulting in the binary cipher.

To decrypt, the XOR operation is repeated between each binary character of the cipher and its corresponding key, resulting in the plaintext in binary.

#### For reference, [One-time Pad](https://en.wikipedia.org/wiki/One-time_pad)
