# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

name : karthick v
reg no : 2122223040086

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
```
mkdir %userprofile%\Desktop\MyLab
```

![image](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/bfd7b36f-4497-4278-a906-314cea739158)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/374033a7-64a6-4884-a60c-72d7245151f4)

![image](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/0559e89f-871d-4f0a-8910-d7795872eeb8)


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```

![image](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/207692f3-fb76-4738-b560-9000d3fee182)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/4d4f1a4f-3650-4f1b-ba15-e9dfae064b8a)

![image](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/22b25a08-844e-47e4-aa38-94add413d6d4)

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```

![image](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/36f087f4-b856-4497-9fe0-7ff7f083746b)


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

![image](https://github.com/karthick-V-212223040086/Windows-basic-commands-batchscript/assets/149037461/274bd337-3663-4266-b469-de96006fa2b9)


# RESULT:
The commands/batch files are executed successfully.

