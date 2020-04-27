## SECTION 1 : PROJECT TITLE
## Temperature Checks for SMEs

<img src="bk/Banner.gif"
     style="float: left; margin-right: 0px;" />

---
## SECTION 2 : EXECUTIVE SUMMARY / PAPER ABSTRACT
When the Circuit Breaker ends and companies start resuming their operation, they will be facing an added task of making sure that employees who have fever don’t turn up for work, and to follow some procedures to handle employees who are now well, and also those who are supposed to be isolated.
In order for companies to determine if employees are sick, one way is to measure their temperature. But not all of them can afford thermal scanners. Also, there would be a lot of administrative work to try to record temperatures for the employees, to identify each one, and to record these employees and their corresponding temperatures in the system.
Hence, we have come up with a low cost system to automate all these processes so that companies can carry out the screening process with minimal manpower and hassle.
This project is meant for SMEs and companies that cannot afford to pay too much to set up the infrastructure to screen employees.
We leveraged tools like UIPath, Python, Google Cloud, the Spring Boot etc to put together a framework for the application.

---
## SECTION 3 : CREDITS / PROJECT CONTRIBUTION


| Official Full Name   | StudentID | Email              | Work Items (Who Did What)                                                                                                  

| CAO LIANG            | A0012884E | e0384184@u.nus.edu | Email module, thermometer reading, architecture diagram, help with integration
| GENG LIANGYU         | A0195278M | e0384909@u.nus.edu | Web GUI, Final Integration, Troubleshooting, Test, Packaging, QA 
| HAN DONGCHOU FRANCIS | A0195414A | e0385045@u.nus.edu | Leading, Requirements and Design, Integration, Reviews, SIT tests 
| ONG BOON PING        | A0195172B | e0384803@u.nus.edu | UIPath, face recognition program and Integration with Temperature Reading                          
| TAN CHIN GEE         | A0195296M | e0384927@u.nus.edu | initial coding of face_recognition.py, report, video, aruco_detect.py   		             
---
## SECTION 4 : VIDEO OF SYSTEM MODELLING & USE CASE DEMO

[Introduction Video]( https://youtu.be/osvUxGM6XUM)


---
## SECTION 5 : USER GUIDE

`<Github File Link>` : <https://github.com/francis-han/Temperature_Checks_for_SMEs/blob/master/ProjectReport/ProjectReport.doc>

### [ 1 ] To run the system in windows or iss-vm

> Prerequisites to run ipa-web

> 1.	Need java8/JRE8 to be installed.

> 2.	Make sure the java/JRE has been added in path env variable(by default, it is there).

> 3.	Make sure UiPath is installed so that user is able to trigger the "start process" properly.

> Files needed:

> 1. config.properties, config file for the UiPath and processes which will be closed during stop processes

> 1.1 uiRobot_path, this need to be updated to user local installation path, like below: 
C:/Users/AppData/Local/UiPath/app-19.12.0-beta0061/UiRobot.exe

> 1.2 temperature_uiPath_file, this need to be updated to sequence.xaml in current project, like below:
C:/Users/Temperature_Checks_for_SMEs/executables/executables/Sequence.xaml

> 1.3 process_list, while user click "stop process", processes configured here will be closed, like WindowsCamera, UiRobot etc.

> The process name might be different due to different machine, so need to configure this manually, otherwise will have to stop process manually.

> 2. employee.csv, includes the employee details input from WebUI.

> 3. known_people, when user upload the employee photo, it will be added into this folder.

> How to start ipa-web

> 1. Go to the ipa-web jar file folder and update the config.properties to reflect the correct file path. For the use of each prop, please refer to above config.properties

> 2. Go the command window and cd to the folder which contains the ipa-web-0.1.0.jar. E.g cd C:\code_repo\Temperature_Checks_for_SMEs\executables\

> 3. Execute below command, and there will be output generated.

> java -jar ipa-web-0.1.0.jar

> 4. Web server started successfully if you see the following output.

> "Root WebApplicationContext: initialization completed in 2832 ms"

> 5. Open any browser and access URL "http://localhost:8090/"

> After opening the browser, you should see the UI 
 

---
## SECTION 6 : PROJECT REPORT 

`<Github File Link>` : <https://github.com/francis-han/Temperature_Checks_for_SMEs/blob/master/ProjectReport/ProjectReport.doc>


