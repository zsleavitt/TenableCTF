# Classic Crypto
## Prompt:
![ClassicCrypto](/images/classic_crypto_prompt.png)

Full value of the crypto (since it ran off the screen):
NzMgNzkgNmUgNzQgN2IgNzAgNjIgNjEgNzQgNjUgNmUgNjcgNjYgNWYgNmMgNjIgNjggNWYgNzQgNjIgNjcgNWYgN2EgNzIgN2Q=

## Tools:
- [Chiper Identifier](https://www.boxentriq.com/code-breaking/cipher-identifier#base64) - "This tool will help you identify the type of cipher, as well as give you information about possibly useful tools to solve it."
- 

## Solution:
I have to admit that cryptography is not my strong suit howeve I did recognize the string as most likely being Base64 crypto where the ciphertext ended in a '=' characters, and mostly contained a combination of upper and lowercase letters. Here is the process I followed to solve this flag:

1. Verified the ciphertext was indeed Base64 by using BoxenTriq:
    1. ![ClassicCrypto1](/images/classic_crypto_1.png)
    1. ![ClassicCrypto2](/images/classic_crypto_2.png)
1. Decoded the ciphertext using the Base64 decoder (again on BoxenTriq):
    1. ![ClassicCrypto3](/images/classic_crypto_3.png)
    1. ![ClassicCrypto4](/images/classic_crypto_4.png)
1. Grabbed the plaintext decoded value and used Cryptii to translate it to text:
    1. ![ClassicCrypto5](/images/classic_crypto_5.png)
1. At this point the 'flag' is starting to look a little bit more recognizable. After recently reading an article about the 'Ceaser Cipher', and remembering that the cifer is merely translating a ASCII character X (typically 13) positions to the right, I whipped out my digits and counted from A to S. Sure enough, 13. Rather than manually traversing the entire string to get the answer I checked out [DCode](https://www.dcode.fr/caesar-cipher):
    1. ![ClassicCrypto6](/images/classic_crypto_6.png)

Flag:
> flag{congrats_you_got_me}