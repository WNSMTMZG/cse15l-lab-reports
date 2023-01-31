## Lab report for incoming cse 15L students 


# How to install VScode on windows:

 *  click on the following link: https://code.visualstudio.com/
 *  after seeing the following image, click on download for windows. It should install automatically 
   ![image](https://user-images.githubusercontent.com/103611867/212757294-52f1186f-007a-4a7c-8f7f-f6a8700253e1.png)
 *  After the install is complete, go to the download folders belonged to your laptop, and install the file you just downloaded
 *  ![image](https://user-images.githubusercontent.com/103611867/212757512-11f13ea4-e209-4e3c-af9a-6696c18f2bc1.png), 
     should be something that look like this
 *  click on it, then click "I accept the agreement" to proceed ---->click next
 *  In the select additional path page, you can choose options that you prefer, there are no right or wrong answers. ---->click next
 *  click install
After that you should see a page that look like this:
![image](https://user-images.githubusercontent.com/103611867/212758087-91a225a8-a9de-4fb7-9576-8b38c040a366.png)
This means you are good to go. Start explooring, Hooray!!! 





# Remotely connecting 

 *  Install git for windows, click on the following link： https://gitforwindows.org/
 *  You should see a page that looks like this, ![image](https://user-images.githubusercontent.com/103611867/212758383-761be574-207f-4873-ad14-17ad501e50bb.png), click on download to proceed
 *  follow the instruction to install git
 *  Open Bash on windows using vscode
 *  enter the following command in your terminal ssh cs15lwi23+your student account+@ieng6.ucsd.edu
 *  If this is the first time you ever opened this terminal, you should see a message as the following: 
 
  The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
  RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
  Are you sure you want to continue connecting (yes/no/[fingerprint])? ----->click on yes

 * 7.After that, you should see the following page if you did it correctly ![image](https://user-images.githubusercontent.com/103611867/212761321-4f3610c3-1fb3-407a-931d-7a4b490d1c10.png)

# Run some commands 
*  Finally, we will be running some commands yourself on the terminal, once you are successfully logged into the remote system. 
*  Try the following commands and see what print out. 
 
  * cd ~
  * cd
  * ls -lat
  * ls -a
  * ls <directory> where <directory> is /home/linux/ieng6/cs15lwi23/cs15lwi23abc, where the abc is one of the other group members’ username
  * cp /home/linux/ieng6/cs15lwi23/public/hello.txt ~/
*  If your result is somewhat similar to the following image, then you are good to go.![image](https://user-images.githubusercontent.com/103611867/212762087-d8d08a85-4f86-4425-abce-3eb92cb9d817.png)
*  what do each of the commands mean? 
   * cd: change current directory 
   * ls: list all files that's in that folder(the current folder)
   * ls -lat: shows all files in your folder/directory including cache files and their detailed information like date intialized or visited and who accessed it
   * ls -a:shows all files in your folder without detailed information. 
   * cp: creates an exact copy of a file in that given location. 

# Congratualations, you have completed this lab 1 tutorial on how to setup vscode and remote connection in a virutal environment!!!!!!
  
  
  



