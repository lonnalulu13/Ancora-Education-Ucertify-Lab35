# Ancora-Education-Ucertify-Lab35
# Performing Symmetric Encryption

Symmetric encryption is a cryptographic technique where the same secret key is used for both the encryption and decryption of data. In this method, the sender and the receiver of the data share a common key that is kept secret. When the sender wants to send encrypted data, they use the secret key to encrypt it. The receiver then uses the same secret key to decrypt and recover the original data.

> **Original Lab Source**
> 
> This lab was available through:
>
> [https://ancoraeducation.ucertify.com/app/?func=navigate_items&item_sequence=8]

## Objective of the Lab
This lab session demonstrates the steps involved in examining symmetric encryption. Upon completion of this lab, you will be able to: 
* Understand the concept of symmetric encryption.
* Perform symmetric encryption.
* Examine the results of symmetric encryption. Lab/Machine Environment You are provided with the Linux virtual machine
## PART A: Encrypting the test.txt file
### STEP 1
From the left sidebar, click the Terminal icon. 
### STEP 2 
Execute the following command to pass the argument in the test.txt file:
```bash
echo Welcome to uCertify! > test.txt
```
### NOTE
The echo command is used to display a line of text/string that is passed as an argument. 
### STEP 3 
Execute the following command to view the content of the test.txt file:
```bash
cat test.txt
```
### STEP 4
Execute the following command to encrypt the test.txt file using a symmetric key:
```bash
gpg -c test.txt
```
GnuPrivacy Guard (GPG) allows you to securely encrypt files so that only the intended recipient can decrypt them. 
### Note 
The gpg -c test.txt command encrypts with a symmetric cipher using a passphrase. 
### STEP 5 
In the Passphrase dialog box, type uc@123456 as passphrase and click OK. 
#### STEP 6 
Execute the following command to view the content of the encrypted test.txt file:
```bash
cat test.txt.gpg
```
## PART B: Decrypting the test.txt file
### STEP 1
Execute the following command to decrypt the encrypted test.txt file:
```bash
gpg -o output.txt test.txt.gpg
```
The decrypted output.txt file will be created with the same content as that of test.txt file. 
### Note 
The gpg -o output.txt test.txt.gpg command decrypts an encrypted file and writes output to the file. 
### STEP 2 
Execute the following command to view the content of the output.txt file:
```bash
cat output.txt
```
### STEP 3 
Close all windows. 
## Lab Summary 
This lab session provides you with a straightforward and practical understanding of performing symmetric encryption. Here's a summary of what you have learned: 
* How to perform symmetric encryption.
* How to examine the results of symmetric encryption.
* How to run cmdlets in Terminal.

Now, you are equipped with the knowledge and skills to perform symmetric encryption.

## Disclaimer

This repository is for **educational and personal learning purposes only**.  

The original lab content belongs to **uCertify / Ancora Education** and remains their copyrighted material.  
This repository is not affiliated with, endorsed by, or sponsored by uCertify or Ancora Education.  

No copyright infringement is intended.  
Use of any tools or techniques mentioned here should only be performed in authorized, legal environments.
