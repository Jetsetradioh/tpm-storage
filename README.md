# tpm-storage
A secure and user-friendly PowerShell tool to manage, encrypt, and decrypt sensitive recovery keys with TPM-based protection. Designed with logs, folder isolation, configurable storage path, and safety-first features.

TPM Manager is a secure and user-friendly PowerShell application to manage, encrypt, and decrypt sensitive recovery keys using Windows' Trusted Platform Module (TPM) capabilities. It includes automatic logging, configurable storage, and supports multiple application profiles.

🔐 Features

🔑 Encrypt and decrypt recovery keys with TPM (CurrentUser scope)

🗂 Create and manage multiple applications' recovery folders

📁 Change default storage location with GUI folder selector

🧠 Remembers chosen storage location via config.txt

🔊 Beep and in-console highlighting for warnings and errors

🧾 Logs stored and auto-rotated in a dedicated Logs folder

❌ Prevents creation of system-reserved folder names like Logs, Temp, etc.

🚀 How to Use

1. Run the App

Use the provided Launch_TPM_Manager.bat file to open the script with the correct settings:

powershell.exe -NoLogo -NoExit -ExecutionPolicy Bypass -File "TPM Manager.ps1"

2. Select Storage Location (First Time Only)

A prompt or GUI will ask you where to store your recovery files.

This path is saved to config.txt automatically.

3. Main Menu Options

1. Manage recovery keys
2. Change storage location
3. Exit

4. Recovery Key Management

Choose or create an application (e.g., "Proton", "Ente")

Encrypt or decrypt the .txt recovery key file

Automatically removes plaintext after re-encryption

📦 Files Included

TPM Manager.ps1 – main PowerShell app

Launch_TPM_Manager.bat – starter file for Windows

tpm_icon.ico – placeholder for optional shortcut icon

README.txt – quick start in plain text

✅ Requirements

Windows OS (PowerShell 5.1+)

TPM available on system (for ProtectedData encryption)

Admin rights not required (runs per user)

💡 Tip

Keep your .ps1 and .bat files in the same folder. You can create a desktop shortcut to Launch_TPM_Manager.bat and assign the icon tpm_icon.ico for a polished experience.

🧠 Credits

Feel free to customize or improve!

