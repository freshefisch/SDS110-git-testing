# SDS110-git-testing

This is a basic readme file. 

#### Here's some math!

$\pi=\frac{22}{7}$

### Python Code Snippet

```python
from string import ascii_lowercase

def substitution_cipher_enc(message, key): # LOWERCASE ONLY
    ciphertext = ""
    for c in message:
        char_id = ascii_lowercase.find(c)
        c_enc = key[char_id]
        ciphertext += c_enc
        # print(c, "->", key[char_id], "|", ciphertext)
    return ciphertext

def substitution_cipher_dec(ciphertext, key):
    message = ""
    for c in ciphertext:
        char_id = key.find(c)
        c_dec = ascii_lowercase[char_id]
        message += c_dec
    return message

c = substitution_cipher_enc("spectacularity", "syofelxkaqbmrznugjpitdhwcv")
m = substitution_cipher_dec("ndejemmauiaosmmc", "syofelxkaqbmrznugjpitdhwcv")
print(c, m)
```
