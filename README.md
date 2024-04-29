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
mkdir %userprofile%\Desktop\MyLab
![Screenshot 2024-04-29 204354](https://github.com/Rogith08/Windows-basic-commands-batchscript/assets/162728044/45442614-e741-405d-b6a6-604da5606b1b)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![Screenshot 2024-04-29 204405](https://github.com/Rogith08/Windows-basic-commands-batchscript/assets/162728044/ccc58969-1259-4298-8f65-7ecd5285c45f)

![Screenshot 2024-04-29 204421](https://github.com/Rogith08/Windows-basic-commands-batchscript/assets/162728044/7cd0d811-7a6a-4e64-875d-1ae76bd74966)


List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab
![Screenshot 2024-04-29 204432](https://github.com/Rogith08/Windows-basic-commands-batchscript/assets/162728044/d1b25b27-9f5f-48a3-b674-8784b5717c99)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
![Screenshot 2024-04-29 204457](https://github.com/Rogith08/Windows-basic-commands-batchscript/assets/162728044/8d74c89e-221b-4aca-a8df-6b9db01644cf)

![Screenshot 2024-04-29 204509](https://github.com/Rogith08/Windows-basic-commands-batchscript/assets/162728044/de8e9730-ada3-40fe-82c2-3dfdb7577a81)

Move the "MyLab" directory to the "Documents" folder.
## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![Screenshot 2024-04-29 204520](https://github.com/Rogith08/Windows-basic-commands-batchscript/assets/162728044/1fafca5b-3a4b-4d13-a9c4-27f78cfed5e7)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT:
![Screenshot 2024-04-29 204535](https://github.com/Rogith08/Windows-basic-commands-batchscript/assets/162728044/b45f2a58-c545-4a1a-847f-f0baf9c7eda7)

# RESULT:
The commands/batch files are executed successfully.

