# Personal_Journal_App

1)PREREQUISITES

a)The application is built up using python 3.7.*.Before running the application, please make sure python 3 is installed. b)Open the readme.txt file in Notepad++ for better visibility.

======================================================================================================================================== 2)ARCHITECTURE

a)Entire application architecture is based upon SOLID principle b)PersonalJournalApp is the parent project.The parent project contains below python packages.All the data in the application is stored in json(JavaScript Object Notation) file as it is light weight and can be supported by most of the high level programming language and web frameworks.

IMPLEMENT_CODE---(Implementation logic is written)

INTERFACE--------(Though python don't have interface concept as it support multiple inheritance,all the functionality are 
				   structured using abstract class)

PROVIDER---------(It contain the "StartFile.py" file , which actually runs the application)

RESOURCES--------(It contain "UsersList.json" in which users are listed.If any how the file is deleted,program will automatically
				  create the file,but in this case earlier registered users will not be available.While creating the UsersList.json, program will add default user "Admin" with password "Admin@123".You can login in the application using the password 
				  and login.Another user "kuntal.barik" is added in the list. You can use the password "kuntal" to login against the user id and taste the case where if maximum no of messages exceeds 50, oldest message will be swapped.
				  
				  Please make sure while testing the above case attached "journalFile.json" file is available 
				  in path "C:\JournalData\kuntal.barik")
NOTE--- Along with the basic feature mentioned in the assessment,additional feature of maintaining log is also added. Log will be printing in "C:\JOURNAL APP LOG" folder as log_YYYY-MM-DD.txt format User Journal message will be saved in "C:\JournalData" folder and per user data will be different.

======================================================================================================================================== 3)TESTCASES

a)All functional testing is done,and test result is positive. b)UserName primary key entity is maintained. c)Password does not contain any "white space".To allow white space in password ,code is commented.You can uncomment the code if you wish. d)Max-message count also tested. In case maximum message exceeds,oldest messages will be swapped with new message e)Logs file can be used to debug the running process of the application.

======================================================================================================================================== 4)INSTRUCTION TO RUN

a)If you are running the program using command prompt/power shell, please please do "extract here\" of the folder "Kuntal Barik.rar" Using cmd/power shell navigate inside the folder.Suppose the folder "Kuntal Barik" is available in your desktop and your user name is XYZ.

Please run below command to navigate inside the folder. cd "C:\Users\XYZ\Desktop\Kuntal Barik\Main Project" (User Name XYZ should be changed according to user name)

Once you are inside "Kuntal Barik\Main Project" folder, please run below command. python -m PersonalJournalApp.PROVIDER.StartFile.py

b)If you want to run the application in any IDE, please do "extract here\" of the folder "Kuntal Barik.rar" and from inside the folder
"Kuntal Barik\Main Project" only open "PersonalJournalApp" with your IDE. Once the folder "PersonalJournalApp" is opened in IDE, open "PROVIDER" folder run "StartFile.py" file.

c)Running using docker is giveniside zip folder

NOTE--Please don't delete """init.py""" file from any where though it is empty. It is required for python package distribution.

========================================================================================================================================
