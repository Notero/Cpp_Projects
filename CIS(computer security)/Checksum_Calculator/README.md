# ✅ Checksum Calculator (pa02)

## 📄 Description
This program computes **checksums** for a given text file in one of three formats:
- **8-bit**
- **16-bit**
- **32-bit**

It reads the input text file, optionally pads it to fit the checksum block size, and prints the formatted checksum output. Padding is done using 'X' characters, and a newline (\n) is always added.

## 📦 Compilation (C++)
    g++ -o pa02 pa02.cpp

## 🚀 Execution
    ./pa02 input.txt checksumsize

# Arguments:
# - input.txt: your input file containing text (a single line)
# - checksumsize: one of 8, 16, or 32

## 📌 Example
    ./pa02 message.txt 16

## 🧪 Sample Output
hellohello

16-bit checksum is 2c97 for all 11 characters

## 📝 Notes
- Adds LF ('\\n') to the input before processing
- Pads with 'X' to ensure full blocks for 16 or 32-bit checksums
- Calculates sum of ASCII values by block and masks final result
- Masks:
  -     8-bit: 0xFF
  -     16-bit: 0xFFFF
  -     32-bit: 0xFFFFFFFF

## 🔐 Academic Integrity
I Akin Korkmaz (ak235142) affirm that this program is entirely my own work and that I have neither developed my code with any another person, nor copied any code from any other person, nor permitted my code to be copied or otherwise used by any other person, nor have I copied, modified, or otherwise used programs created by others. I acknowledge that any violation of the above terms will be treated as academic dishonesty.
\`\`\`
EOF
