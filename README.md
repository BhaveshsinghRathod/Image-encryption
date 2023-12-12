# Image-encryption
Image encryption refers to the process of encrypting an image so that the content can be hidden from the viewer. In order to view the encrypted image, the image first needs to be decrypted.
There are numerous methods and algorithms available to use for the encryption and decryption purpose. 
The keys used in the encryption and decryption algorithms are broadly classified into 2 categories. They are
  1) Symmetric key and
  2) Asymmetric key
Symmetric key:
  If the key used for decryption is the same key that was used for         
  encryption purpose, then the key is said to be symmetric key.
Asymmetric key:
  If the key used for encryption and decrytion are different then that key 
  is called as asymmetric key.


Explanation of the code:

**Understanding of the imported classes**
All the necessary classes are imported from their respective pacakages.
The Cipher class is an important part of the cryptographic operation in java. It mainly provides different functionalities for encryption and decryption using different algorithms such as "AES", "ECB" etc.
We need to construct a secret key from a byte array, for that we use SecretKeySpec.
The io.File class imported will be used for representing the file path in the system.
io.FileInputStream is used to read data from a file for encryption purpose.
io.FileOutputStream is used to write encrypted data to a file.

**Basic working of the code**
The system will first generate a 128 bit key i.e. a 16 character key for the encryption and decryption process.
The system will now ask for the path to file and create 2 new file where it will be storing the "encrypted" and the "decrypted files" respectively.
The "encrypt" and "decrypt" methods will start the process of encryption and decryption respectively. 
The "doCrypto" method will initialize a secret key and then create a "cipher" instance with the help of AES algorithm. It will then read the data or the contents of the input file into a byte array and will later write results to the output file after performing encryption or decryption on that byte array.
