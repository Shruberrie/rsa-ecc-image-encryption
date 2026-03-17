# Layered Image Encryption using RSA and ECC

Overview

This project implements layered image encryption using two public-key cryptographic algorithms:

1. RSA
2. Elliptic Curve Cryptography (ECC)

The input image is first encrypted using RSA. The resulting image is then encrypted again using ECC. Decryption reverses the process by first applying ECC decryption followed by RSA decryption.

Encryption Pipeline

Original Image
↓
RSA Encryption
↓
RSA Encrypted Image
↓
ECC Encryption
↓
Final Encrypted Image

Decryption Process

Encrypted Image
↓
ECC Decryption
↓
RSA Decryption
↓
Original Image

Technologies

Python  
NumPy  
OpenCV  

Project Structure

src/ → encryption algorithms  
images/ → input images  
results/ → encrypted outputs  
notebook/ → project notebook  

Running the Project

Install dependencies

pip install -r requirements.txt
