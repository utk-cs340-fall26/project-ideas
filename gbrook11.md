# PassFile - Locally Stored and Secure Password and File Manager

---

This project is focused on providing a secure, locally stored application that stores passwords and sensitive documents. 
It will use an encrypted and cryptographically secured file to store the passwords and provide a directory to store any sensitive documents. Access to inserted information will be safeguarded with a master password the user provides upon initial startup.
After providing the master password, the user can temporarily view and copy their passwords and files that they have put into the application. Utilizing timers and a temporary clipboard, we can remotely delete the clipboard after a set time to maintain security related to these.

# Solutions for Problems and their People 

---

Creating secure passwords that don't repeat themselves can be a time consuming process that creates seemingly unnecessary, to the point that most people don't do it and opt for short, weak, and repeated passwords.
This is a massive security issue, as it allows brute force attacks to have great effectiveness. 
Additionally, if a data breach occurs on another web service, it allows an attacker to log into some other web service using the same password.
PassFile will help allow its users to create strong, once-per-account passwords and have a repository to recall their passwords.
Additionally, finding files on a computer without an organization plan can be agonizing, especially when they can be distributed throughout multiple directories on the system.
Having a secure, centralized hub for sensitive files will assist with and ensure that bad actors can’t obtain access.
This application is intended for those who want to ensure their digital footprint is secure while not losing access to their accounts.

# Major Features

---

- Secure Passwords and Files
- Enhanced Cryptography for sensitive files
- Organize sensitive information within a centralized hub

# Tools for the Trade

---

For this project, we plan to use C++ for the entire project, with QT 6 for the GUI elements, Botan for the cryptography angle, and libsodium for memory handling.

