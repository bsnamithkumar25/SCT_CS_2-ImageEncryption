# Image Encryption Tool – Pixel-Level Security in Python

SkillCraft Cybersecurity Internship – Task 2  
Author: B S Namith Kumar  
Domain: Cybersecurity

---

## Project Overview

This is a Python-based image encryption and decryption tool developed for Task 2 of my internship at SkillCraft Technology. It manipulates pixel data using simple but effective methods to distort and restore images.

## Features

- 🔐 Encrypt and decrypt any `.jpg` or `.png` image  
- Two reversible techniques:
  - Pixel Swap
  - Mathematical Pixel Transformation
- Command-line interface (CLI) with arguments for easy control  
- Folder-structured workflow for automation

---

## Learning Outcomes

- Understood fundamentals of image obfuscation techniques  
- Manipulated image pixels with NumPy and PIL  
- Built modular CLI tools using `argparse`  
- Practiced reversible encryption logic  
- Gained hands-on experience with image processing in cybersecurity

---

## Sample Run

### Encrypt Image Using Pixel Swap
```bash
python main.py encrypt input/sample.jpg output/encrypted_swap.jpg --method swap
```
 Effect: Adjacent pixels are swapped, making the image unrecognizable.

---

###  Decrypt Image Using Pixel Swap
```bash
python main.py decrypt output/encrypted_swap.jpg output/decrypted_swap.jpg --method swap
```
📷 Effect: The original image is fully restored.

---

###  Encrypt Image Using Math Operation
```bash
python main.py encrypt input/sample.jpg output/encrypted_math.jpg --method math
```
📷 Effect: Each pixel value is modified by adding a constant (default `+50`).

---

###  Decrypt Image Using Math Operation
```bash
python main.py decrypt output/encrypted_math.jpg output/decrypted_math.jpg --method math
```
 Effect: The same constant is subtracted, restoring original image.

---

##  Notes

- Only RGB images (.jpg, .png) supported  
- Create two folders:  
  - `/input` for source images  
  - `/output` for encrypted/decrypted results  
- Default math constant is `+50`, changeable in code  
- Spaces in file names are not recommended  
- Run with Python 3 and install dependencies using:  
```bash
pip install pillow numpy
```


- [SkillCraft Task Portal](https://skillcraft-technology-tasks.my.canva.site/)

---

> Classical problems need modern thinking. This project proves that even with basic tools, secure encryption is achievable.
