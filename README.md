# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 

# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-11 043824](https://github.com/user-attachments/assets/fa5fd9dc-1ad7-4b2d-a5c8-3f2f7dc23449)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/4f7f3143-bfc5-4a54-b0ee-2c915e38521b)

```
type nul > MyFile.txt
```
![Screenshot 2025-05-11 044131](https://github.com/user-attachments/assets/168cab9c-91ae-43de-bf75-167665bec993)

List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-11 044340](https://github.com/user-attachments/assets/7af416c3-bee4-4b9e-ab70-f422694ef5e0)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/c98f2fed-1a0b-4a05-b8fc-ac0311bb2670)
```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/d6c58ab4-c395-4df5-85b9-dac4a4c44751)

Move the "MyLab" directory to the "Documents" folder.
## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
```
![image](https://github.com/user-attachments/assets/95e12e5f-e5f0-4033-94ad-c15d10ad4e7e)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
## OUTPUT
![image](https://github.com/user-attachments/assets/67a54364-2082-4642-9c0b-5ee7820c88c2)

COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT

![image](https://github.com/user-attachments/assets/60c22d48-276e-46ea-8070-c32d2737a664)

# RESULT:
The commands/batch files are executed successfully.

