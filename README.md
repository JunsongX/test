# Xterm GUI

Here is a document of how to use the Xterm GUI, with each button's function and how it works.

## FTP PUT Tab

This tab is used for put file into the remote server. It has two parts: put single file or mirror the entire folder to the remote folder.

**To get started, first you need to input your login information(username and password) into the system.**
Below will be each button's function and the require information to use it.

### Select location of file to FTP
This button allow you to choose the file you want to transfer to the remote server in your local machine. Once you choose the file, the file path will be shown in the left **Local file** space.

### Make Folder on ftp_3d
This button helps to make a folder in the remote server's **ftp_3d** folder. To use it, first you need to input the folder name you want to create in gthe **Remote folder** space, then click the button and the folder will be made in ftp_3d folder.

### FTP PUT Single file
This button works when you have single file to put into the remote server. Required information: Login information(username and password), **Local file** location,
**Remote folder** name. If you did not make a folder before clicking the FTP PUT Single file button, the file will automatically saved in the path **ftp_3d/user_name**. 

To put the file in an already exist folder, just write the exist folder name in the **Remote folder** space and **DO NOT** click the Make folder button.

### Mirror the Entire folder to ftp_3d
This button works when you have a whole folder to put into the remote server. Required information: Login information(username and password), **Local file** location,
**Remote folder** name. To use this function first you need to choose the file by using the **Select location of file to FTP** button to choose file, and input the folder name in **Remote folder** space.

**Example**: you choose the gds file and the path shown is "/home/user/LCC/test.db", and you made a folder called "Xterm" in ftp_3d. Then **all the file in LCC folder** will be copied to the Xterm folder in ftp_3d.

### Show FTP content
This button will show you all the thing in the Remote server after you login, and if you click the content, the path will show in the **Remote Path** status box.

## Vis Generation Tab
This tab is used for vis file generation, with input the required information, it will create a vis file directly.

### Get .vis File
This button let you choose the vis template location, all the further edit will based on the template you choose here. After choose the template, the path information will be shown on the left **VIS TEMPLATE LOCATION** space.

### Get gds path from FTP PUT
**IMPORTANT**: to get the correct information, you will need the FTP PUT tab's information.

Please use the FTP PUT tab's **Select location of file to FTP** button to choose the gds file you need in your vis file. Use the **Remote folder** space to choose the path after "home/santos3d/ftp/username/", and then when you click the **Get gds path from FTP PUT**, the path will become **home/santos3d/ftp/username/Remote folder/vis file you choose in ftp put**.

### Create modified .vis File
This button will require you to input the window information in X1, Y1, X2, Y2, output path(if blank will use default path), output name(if blank will use default file name) and name of new vis file. After clicking the Create button, the local path of the new vis file will be shown in below status box, and you can go to that path and find your new new generated vis file.

## FTP Get Tab
**To get started, first you need to input your login information(username and password) into the system.**

### Select location of folder to get file
This button allow you to select which local path you would like to contain the mirror folder.

### Choose file to get 
This button will show you the remote content after login, you can go to yukan_3d/work_dir/username to find the folder you want to get back, by click the folder name, the path will shown in **Remote Path** space. **IMPORTANT**: Please choose folder instead of just choose single file.

### FTP Get file
By click this button, the whole folder will be get back.

**Example**: The local folder you choose is "/home/user/LCC", and the Remote folder you choose to mirror back is "/yukan_3d/FCC_WORKbics8/username/test_folder", then when you click the **FTP Get file** button, all the content of test_folder will get back, and the final path is "/home/user/LCC/test_folder"(you do not need to create folder by yourself).
