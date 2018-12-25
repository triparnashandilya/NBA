# NBA-Accreditition Report Generator
### The system generates the report of NBA accreditation
This is an application intended for college faculty members to ease the process of generating NBA report by taking input from faculty and student. 
Generating Accreditation,matching CIF outcome with program outcome,taking feedback from students on their program outcome, taking indirect feedback from teacher etc
### Input
(a) Student feedback (Feedback about the level of course outcome attained.)<br/>
(b) Marks List (Scores of students of a course for particular batch.)<br/>
(c) CO List (Course outcome for a course.)<br/>
(d) PO List (Program outcome for a course.)<br/>
(e) Correlation Matrix (Correlation between CO and PO)<br/>
(f) CO vs AC (Assessment Component) Details<br/>
### Tools and Technologies
Development Tool: Eclipse Oxygen<br/> 
API: Apache POI <br/>
Web server tool: Apache Tomcat <br/>
Skills Used: Java, HTML ,CSS <br/>
### Output
(a) NBA Accreditation Report containing course code table(from direct feedback) and end of course survey table(indirect feedback).
### Constraints
(a) All student may not fill feedback form.<br/>
(b) Faculty has to provide details ( like Excel Sheets) in the format as mentioned.<br/>
(c) In the marks list the entries of marks is of only integer type.<br/>
### Process
(a) Procedure of generating NBA Report<br/>
(b) Calculating Success % for each Assessment Component for corresponding to each course. <br/>
(c) Calculating Direct Weight from direct feedback obtained.<br/>
(d) Calculating weighted sum for CO with respect to AC for every course.<br/>
(e) Calculating indirect weight and generating course code table(from direct feedback) and end of course survey table(indirect feedback).<br/>
### GUI
Home page<br/>
Faculty Login<br/>
Student Login<br/>
About Us<br/>
Upload pages for CO and PO statements, marks, CO/AC and correlation matrix.<br/>
Feedback Form page.<br/>

### Dependencies


#### Step 1: Install Java JDK8
You must have Java installed on the system before installing Apache Tomcat on a Linux VPS. Tomcat 9 required Java 8 or later version to work. You can check and verify that Java is installed with the right version.

java -version

java version "1.8.0_144"
Java(TM) SE Runtime Environment (build 1.8.0_144-b01)
Java HotSpot(TM) 64-Bit Server VM (build 25.144-b01, mixed mode)

If you don’t have Java installed on your system or installed a lower version, run below commands to satisfy requirements.

sudo apt-get update
sudo apt-get install default-jdk
sudo add-apt-repository ppa:webupd8team/java
sudo apt update
sudo apt install oracle-java8-installer
#### Step 2: Download Eclipse Oxygen
Now that Java JDK 8 is installed, got and download Eclipse Oxygen IDE package for your systems.. the link below can be used to get it.

https://www.eclipse.org/downloads/

#### Step 3: Install Eclipse IDE

Use the commands below to extract the content in the  ~/Downloads folder… The next line launches the installer…

tar xfz ~/Downloads/eclipse-inst-linux64.tar.gz
~/Downloads/eclipse-installer/eclipse-inst

for the packages you need to install to have eclipse IDE for java EE developers 
Use the onscreen instructions to complete the installer.. Accept the default installation directory and continue

Right click on project
build path
Add external archives


https://dev.mysql.com/downloads/connector/j/
platform independent

mysql-connector-java-8.0.13.zip
Download Link: https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-8.0.13.zip

#### Step4 Install Tomcat
<br/> <b>Step1</b> Download Tomcat From here: http://mirrors.estointernet.in/apache/tomcat/tomcat-7/v7.0.92/bin/apache-tomcat-7.0.92.tar.gz
<br/> <b>Step2</b> Extract the tar file
<br/> <b>Step3</b> Now make a directory at usr/local/tomcat <br/> sudo mkdir /usr/local/tomcat
<br/> <b>Step4</b> move the extracted file to the directory <br/> sudo mv apache-tomcat-7.0.92 /usr/local/tomcat
<br/> <b>Step5</b> Move to that directory <br/> cd /usr/local/tomcat <br/> cd /usr/local/tomcat/apache-tomcat-7.0.92
<br/> <b>Step6</b> Run these commands <br/> sudo ln -s /var/lib/tomcat7/conf conf <br/> sudo ln -s /tc/tomcat7/policy.d/03catalina.policy/conf/catalina.policy <br/> sudo ln -s /var/log/tomcat7 log <br/> sudo chmod -R 777 /usr/local/tomcat/apache*/conf <br/>
<br/> <b>Step7</b> Configuring the Server <br/> 1  From the Eclipse main menu choose File > New > Other...<br/> 2  Select Server > Server.<br/> 3  Click Next. <br/> 4  Select Tomcat vx.x Server<br/> 5  Click Next. <br/> 6  Browse to the folder of your Tomcat installation. (or type /usr/local/tomcat/apace-tomcat-7.0.92)<br/> 7  Select Finish.<br/>

### Code
<br/> 1 File->New->Dynamic Web Project
<br/> 2 Write Project Name
<br/> 3 In your project in JavaScript Resources right click in webContent new JSP File

### References
https://websiteforstudents.com/how-to-install-eclipse-oxygen-ide-on-ubuntu-167-04-17-10-18-04/ <br/>
https://www.youtube.com/watch?v=D0OfTZuIDcs <br/>
https://help.eclipse.org/neon/index.jsp?topic=%2Forg.eclipse.stardust.docs.wst%2Fhtml%2Fwst-integration%2Fconfiguration.html <br/>
https://www.youtube.com/watch?v=HYSrsxhyEik&index=34&list=PLsyeobzWxl7pUPF2xjjJiG4BKC9x_GY46 <br/>
https://www.codejava.net/java-ee/servlet/eclipse-file-upload-servlet-with-apache-common-file-upload <br/>
https://www.journaldev.com/1964/servlet-upload-file-download-example <br/>
https://www.quora.com/How-do-I-create-a-basic-login-and-register-page-in-HTML <br/>


#### ER Diagram

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/ER%20Diagram.png" width="500" title="hover text">
</p>


#### Class Diagram

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/Class%20Diagram%20for%20NBA%20Accreditation%20.png" width="500" title="hover text">
</p>

## ScreenShot

### Home Page

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/Home.png" width="500" title="hover text">
</p>

## Faculty

### Faculty Login

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/facultyLogin.png" width="500" title="hover text">
</p>

### Faculty Page

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/facultyPage.png" width="500" title="hover text">
</p>

### Faculty

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/faculty.png" width="500" title="hover text">
</p>

### Upload CO/AC List

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/COAC.png" width="500" title="hover text">
</p>


### Upload COList

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/COList.png" width="500" title="hover text">
</p>

### Upload Correlation matrix

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/CorrelationMatrix.png" width="500" title="hover text">
</p>






### Upload POList

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/POList.png" width="500" title="hover text">
</p>

### Upload Marks

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/marks.png" width="500" title="hover text">
</p>

## Student

### Student Login Page

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/studentLogin.png" width="500" title="hover text">
</p>

### Student Page

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/studentPage.png" width="500" title="hover text">
</p>

### Student Feedback

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/studentFeedback.png" width="500" title="hover text">
</p>



### NBA Report

 <p align="center">
  <img src="https://github.com/Parulshandilya/NBA-Accreditition-Report-Generation/blob/master/images/NBAReport.png" width="500" title="hover text">
</p>



