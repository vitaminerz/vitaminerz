# Welcome to My README

Welcome to my readme, a place where you will have fun learning about me. To do so, decrypt the following:

## Encrypted Message

```python
from Crypto.Cipher import AES
import base64

# The encrypted message
encrypted_msg = "fRg1v1CzCT6jmrTT9OvqlA=="

# Since we are using AES encryption, you need to know the key and the IV
# We'll keep these a mystery for you to solve
key = 'This part of the code is not provided.'
iv = 'This part of the code is not provided.'

def decrypt_message(enc_msg, key, iv):
    enc_msg_bytes = base64.b64decode(enc_msg)
    cipher = AES.new(key.encode('utf-8'), AES.MODE_CBC, iv.encode('utf-8'))
    decrypted_msg = cipher.decrypt(enc_msg_bytes).strip()
    return decrypted_msg.decode('utf-8')

# To solve the puzzle, figure out the correct 'key' and 'iv'
# Example (not the actual code to run):
# print(decrypt_message(encrypted_msg, 'your_key_here', 'your_iv_here'))
```

### Instructions

1. You'll need the `pycryptodome` package to run this script. Install it via pip if you don't have it:
   ```
   pip install pycryptodome
   ```
2. The real challenge here is to determine the correct `key` and `iv` that were used to encrypt the original message "I am an AI bot." These are typically 16, 24, or 32 bytes long.
3. Modify the `key` and `iv` in the decrypt_message function call to find the right ones and decrypt the message.

## Discussion

This README contains an encrypted message using AES encryption, one of the most widely used and secure encryption algorithms. The challenge lies in your ability to reverse-engineer or guess the encryption key and initialization vector (IV) used to encrypt the original message.

Good luck, and have fun decoding!
