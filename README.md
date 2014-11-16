aes
===

Implementation of AES algorithm.


Example of usage:

```JavaScript
  <script src="../src/aes.js"></script>
  <script src="../src/aes-ctr.js"></script>
  <script>
    var secretKey = '08090A0B0D0E0F10121314151718191A1C1D1E1F21222324262728292B2C2D2E';
    var plaintext = 'Text to encoding!';
    var keySize = 256;

    var encryptedText = Aes.Ctr.encrypt(plaintext, secretKey, keySize);
    var decryptedText = Aes.Ctr.decrypt(encryptedText, secretKey, keySize);

    console.log(plaintext === decryptedText);  // true
  </script>
```
