# SecureFileSystem

A Python GUI-based application that allows users to **securely compress and encrypt files** using two efficient methods:

- 🗜️ **Huffman Compression**
- 🔐 **AES Encryption**

Built with **`tkinter`** for simplicity, this tool enables users to easily:
- Select input/output files
- Choose operations (Encrypt, Decrypt, Compress, Decompress)
- Enter passwords for encryption
- Get feedback via progress alerts and error messages

---

## 🚀 Features

- ✅ GUI interface (built using `tkinter`)
- ✅ Supports 4 operations:
  - Huffman Compression
  - Huffman Decompression
  - AES Encryption
  - AES Decryption
- ✅ Clean layout with file browsing and password fields
- ✅ Progress/status alerts using `messagebox`
- ✅ Portable design (calls external `.exe` tools)

---

## 🧰 Requirements

- Python 3.x
- tkinter (bundled with Python)
- Two compiled executables:
  - `encrypt_tool.exe` – performs AES encryption/decryption
  - `huffman_cli.exe` – performs Huffman compression/decompression

> These executables are **not written in Python**, so make sure they exist in the same directory as `gui.py`.

---

## 🛠 How to Run

```bash
python gui/gui.py
Make sure encrypt_tool.exe and huffman_cli.exe are in the same directory as gui.py. The GUI won't work without them.

⚙️ Operations
Operation	Description	Executable
Compress	Compresses file using Huffman Coding	huffman_cli.exe
Decompress	Restores original file from compressed one	huffman_cli.exe
Encrypt	Encrypts file using AES + password	encrypt_tool.exe
Decrypt	Decrypts file using AES + password	encrypt_tool.exe

🔐 AES Encryption
Password is passed securely to encrypt_tool.exe

You must enter a password to run encryption/decryption

AES key/IV handling is done inside the compiled tool

🧪 Testing
Use test_files/sample.txt to try compression and encryption.

Output files will be saved where you specify using the GUI.

📝 License
MIT License © 2025 Sourav Gupta
Feel free to use, modify, and distribute.

🙋‍♂️ Author
Sourav Gupta
B.Tech CSE, 4th Semester
Graphic Era University, 2025
