# Name : Tarun S
# Reg no : 212223040226
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
![image](https://github.com/Tarun-2006/Windows-basic-commands-batchscript/assets/145584190/ac9a374c-e4bd-463c-aa79-5032b76f787e)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/Tarun-2006/Windows-basic-commands-batchscript/assets/145584190/faeb40d8-8b27-4af8-a855-d0840e13d7e3)
![image](https://github.com/Tarun-2006/Windows-basic-commands-batchscript/assets/145584190/bcad6ca7-64ac-4e7e-9a82-964cea1b5a2c)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Tarun-2006/Windows-basic-commands-batchscript/assets/145584190/a9e4023a-710d-4e62-8ddf-5e8d9f78ee31)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/Tarun-2006/Windows-basic-commands-batchscript/assets/145584190/47905eda-ecba-4ea2-8dfc-3fd49e7c76ac)
![image](https://github.com/Tarun-2006/Windows-basic-commands-batchscript/assets/145584190/47ee6ae7-bcab-43e1-9de3-fe7412a455e8)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/Tarun-2006/Windows-basic-commands-batchscript/assets/145584190/fa90727b-f07a-4d3f-8ee5-7b7a6819836e)

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




## OUTPUT

![image](https://github.com/Tarun-2006/Windows-basic-commands-batchscript/assets/145584190/13adbdc7-a9c1-499c-92ec-65585c86a11c)




# RESULT:
The commands/batch files are executed successfully.


