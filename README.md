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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
mkdir "C:\Users\admin\Documents\mylab"
```
![image](https://github.com/user-attachments/assets/1dbfa7f8-0ee9-4a2f-842c-313e99d825d3)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd "C:\Users\admin\Documents\mylab"
```
![image](https://github.com/user-attachments/assets/a6e3d2ff-3949-4458-8074-c47498a304e7)

```
type nul > MyFile.txt
```
![image](https://github.com/user-attachments/assets/89a8a3f0-d021-43f6-ab5a-cdad8e153391)

## COMMAND AND OUTPUT
```
dir "C:\Users\admin\Documents\mylab"
```
![image](https://github.com/user-attachments/assets/5dce44bd-46fd-423b-87ec-d39622fbd9a7)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
```
mkdir C:\Users\admin\Documents\backup
```
![image](https://github.com/user-attachments/assets/8f5ff67a-194e-42b2-bd4b-9329f7db573c)
```
copy myfile.txt C:\Users\admin\Documents\backup
```
![image](https://github.com/user-attachments/assets/33fc409a-0474-485a-8840-b90f20f5cc58)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
```
move mylab Document
```
![image](https://github.com/user-attachments/assets/d5b30671-685d-48ac-874f-ba9a8fc08d53)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\DocBackup\*.docx
```
```
BackupScript.bat
```


## OUTPUT

![image](https://github.com/user-attachments/assets/25af0f2a-1726-4991-96b9-b2b5e58feebb)




# RESULT:
The commands/batch files are executed successfully.

