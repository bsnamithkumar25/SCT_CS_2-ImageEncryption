# 🖼️ Simple Image Encryption Tool
**Author:** B S Namith Kumar  
**Internship:** SkillCraft Technology | Cybersecurity Track  
**Task 2:** Develop an image encryption tool using pixel manipulation techniques.

---

## 📌 Description

This Python-based tool performs basic encryption and decryption on images using two techniques:

1. 🔁 **Pixel Swapping**: Swaps adjacent pixels to scramble the image.
2. ➕ **Math Operation**: Adds a constant to each pixel value (mod 256) for reversible encryption.

Both methods are easily reversible and demonstrate how even basic transformations can offer insight into how encryption operates at a pixel level.

---

## 🚀 Features

- Encrypt and decrypt `.jpg`, `.png`, and other RGB images.
- Two techniques: `swap` and `math`
- Clean CLI with `argparse` interface

---

## 🛠️ How to Use

### Encrypt an image:

```bash
python main.py encrypt input/sample.jpg output/encrypted.jpg --method swap
