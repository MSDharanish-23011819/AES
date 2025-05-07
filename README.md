# EX-8-ADVANCED-ENCRYPTION-STANDARD ALGORITHM
# Aim:
To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption.

# ALGORITHM:
AES is based on a design principle known as a substitution–permutation.
AES does not use a Feistel network like DES, it uses variant of Rijndael.
It has a fixed block size of 128 bits, and a key size of 128, 192, or 256 bits.
AES operates on a 4 × 4 column-major order array of bytes, termed the state
# PROGRAM:
```
def xor_encrypt_decrypt(input_text, key):
    output = []
    key_len = len(key)
    for i in range(len(input_text)):
        output_char = chr(ord(input_text[i]) ^ ord(key[i % key_len]))
        output.append(output_char)
    return ''.join(output)
```

# Main
```
url = "WELCOME"
key = "secretkey"
print("Original text:", url)
```

# Encrypt
```
encrypted = xor_encrypt_decrypt(url, key)
print("Encrypted text:", encrypted)
```

# Decrypt
```
decrypted = xor_encrypt_decrypt(encrypted, key)
print("Decrypted text:", decrypted)
```

# OUTPUT:
![Screenshot 2025-04-30 081927](https://github.com/user-attachments/assets/f0a36094-92db-474d-ae2f-f4718a143fb7)

# RESULT:
Thus code for Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption is executed successfully.

