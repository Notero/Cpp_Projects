cat << 'EOF' > README.md
# 🔐 Hill Cipher Encryption Tool (pa01)

## 📄 Description
This program encrypts a plaintext file using the **Hill Cipher** algorithm with a key matrix provided in a key file. It supports:
- Key sizes from **2x2** up to **9x9**
- Removing all punctuation and non-alphabetic characters
- Automatic **lowercasing** of all letters
- Padding with `'x'` if the message length isn’t a multiple of the key size

## 🔧 Usage
To compile and run this assignment (`pa01`) in any of the supported languages:

### C++
    g++ -o pa01 pa01.cpp
    ./pa01 kX.txt pX.txt

Where:
- `kX.txt` is the **key matrix file**
- `pX.txt` is the **plaintext message file**

## 📥 Input Format

### Key File (`kX.txt`)
    3
    6 24 1
    13 16 10
    20 17 15

- First line is the matrix size `n` (e.g., `3`)
- Followed by `n x n` integers for the matrix

### Plaintext File (`pX.txt`)
    Attack at dawn! Retreat if needed.

- May contain punctuation, whitespace, numbers (all of which are ignored)

## 📤 Output
Shows the following:
1. Key Matrix
2. Processed Plaintext (no punctuation or spaces)
3. Encrypted Ciphertext

Both outputs are formatted in **80-character lines** for readability.

## ✍️ Notes
- Only lowercase letters `a-z` are retained for processing.
- Output characters are mapped via modulo 26 arithmetic using the Hill cipher rule.

## 🔒 Academic Integrity
Includes integrity statement confirming that all work is the author's original creation, per CIS3360 academic policy.

---

👨‍💻 **Author**: Akin Korkmaz  
📅 **Created**: September 26, 2024  
📚 **Course**: CIS3360 – Security in Computing – Fall 2024  
🎓 **Instructor**: McAlpin
EOF
