# Encryption-Decryption System using Tkinter and a Modified RC4 Algorithm

This project implements a simple encryption-decryption system built on the Tkinter platform, utilizing a modified version of the RC4 algorithm.

## Key Steps Involved

### Key Scheduling (KSA)
The `Key_Scheduling()` function initializes the S-box using a permutation of the key.

### Pseudo-Random Generation Algorithm (PRGA)
The `stream_generation()` function generates the keystream dynamically.

### Encryption Process
1. The keystream is generated using the standard RC4 mechanism.
2. The encryption modifies only alphabetic and numeric characters:
   - **Letters (A-Z, a-z)** are shifted using the keystream but remain within the English alphabet.
   - **Numbers (0-9)** are also shifted using the keystream but remain within the range of 0-9.
   
This approach differs from traditional RC4, where the plaintext is XORed byte-by-byte with the keystream.

