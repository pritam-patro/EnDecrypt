Simple encryption-decryption system made on tkinter platform with encryption algorithms like a modified version of RC4.
The main steps involved is as follows:
Key Scheduling (KSA): The Key_Scheduling() function initializes the S-box using a permutation of the key.
Pseudo-Random Generation Algorithm (PRGA): The stream_generation() function generates the keystream dynamically.
Encryption Process:
The keystream is generated using the standard RC4 mechanism.
The encryption modifies only alphabetic and numeric characters:
Letters (A-Z, a-z) are shifted using the keystream but remain within the English alphabet.
Numbers (0-9) are also shifted using the keystream but remain within the range of 0-9.
This is different from traditional RC4, where the plaintext is XORed byte-by-byte with the keystream.
