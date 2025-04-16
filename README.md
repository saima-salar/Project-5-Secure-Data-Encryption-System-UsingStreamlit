# Project-5-Secure-Data-Encryption-System-UsingStreamlit
GIAIC
🔐 Secure Multi-User Data System
This is a Streamlit-based application that allows multiple users to securely register, login, and store/retrieve their personal data using end-to-end encryption.

🚀 Features
User Registration & Login

Unique username and password for each user

Passwords are securely hashed using PBKDF2-HMAC with a salt

Lockout Protection

Locks out users for 60 seconds after 3 failed login attempts

Secure Data Storage

Users can encrypt and store their own data with a passphrase

Data is encrypted using Fernet symmetric encryption

Data Retrieval

Users can view encrypted entries

Decrypt data using the same passphrase used during encryption

🛠️ Technologies Used
Streamlit – for the UI

cryptography – for secure encryption/decryption

hashlib – for password hashing

json – for data storage

os, time – for session handling and lockout

📁 Data Storage
All user credentials and encrypted data are saved locally in a file named secure_data.json.

🧪 How to Run
Clone the repo or copy the script

Install dependencies:

pip install streamlit cryptography

streamlit run your_script_name.py

📌 Note
Keep the encryption passphrase safe. Without it, data cannot be decrypted.

Ensure the SALT and secure_data.json are kept confidential for production use.

