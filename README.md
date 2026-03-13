🔐 Password RECAP v2.0

    

Password RECAP v2.0 is a simple multithreaded NTLM hash cracker written in Python. It checks hashes against a wordlist and saves cracked passwords to a result file.


---

⚡ Features

NTLM hash cracking

Multithreaded processing

Fast dictionary attacks

Reads hashes from file

Saves results automatically

Simple CLI interface



---

🧠 How It Works

1. Load hashes from a file


2. Load a wordlist


3. Convert each word to NTLM hash (MD4 UTF-16LE)


4. Compare with target hashes


5. Save results to result.txt




---

📦 Requirements

Python 3.x


Required modules:

hashlib
threading
queue
sys

(All included in Python standard library)


---

📂 Project Structure

project/
│
├── recap.py
├── hashes.txt
├── wordlist.txt
├── result.txt
└── README.md


---

🚀 Usage

Run the script:

python recap.py

Then provide:

Enter hash file path:
Enter wordlist file path:

Example:

Enter hash file path: hashes.txt
Enter wordlist file path: rockyou.txt


---

📄 Example Hash File

8846F7EAEE8FB117AD06BDD830B7586C
32ED87BDB5FDC5E9CBA88547376818D4


---

📄 Example Output

Found password: 'password' for hash: 8846F7EAEE8FB117AD06BDD830B7586C
Found password: '123456' for hash: 32ED87BDB5FDC5E9CBA88547376818D4

Saved to:

result.txt


---

⚠️ Disclaimer

This tool is intended for educational purposes and security testing only.

Do not use it on systems you do not own or have permission to test.


---

👨‍💻 Author

sky


---

⭐ Support

If you like the project:

⭐ Star the repository 🍴 Fork it 🐛 Report issues
