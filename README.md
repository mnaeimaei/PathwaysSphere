# PathwaysSphere

Steps for installing and using the tools

**Step1** Download the test dataset
The dataset name is EventLog.xlsx that can be download in the dataset directory of the repo, you can load this file locally and from google drive.
1. For locally, just put in a directory of your pc, It is recomended to put EventLog.xlsx in Download directory.
2. For google drive, you need to go to Google Cloud Console (https://console.cloud.google.com/). 
Click on the project dropdown next to the Google Cloud Platform logo at the top left. Click on “New Project,” give it a name, and click “Create. 
Navigate to the “APIs & Services > Dashboard” section in the Cloud Console. Click “+ ENABLE APIS AND SERVICES” at the top. Search for “Google Sheets API,” select it, and click “Enable.”
In the Google Sheets API page, click on “Create Credentials”. Choose “Google Sheets API”, select “Web server (e.g., node.js, Tomcat)”, and for “Data will be accessed” choose “Application data”. Click “What credentials do I need?”
You’ll be prompted to create a service account. Set the service account name and description. Click “Create”. Then set the role to “Editor” or any other role that suits your needs (Editor allows read and write access to the API).
After creating the service account, click “Done”. Go to the “Credentials” tab, find your new service account, and click on it. In the service account details, click “Add Key,” then “Create new key.” Choose “JSON” as the key type and click “Create.” This will download a JSON file to your computer.
Then upload the excel file in the google drive after uploading the file in your google drive, Open it. Click on “Share” in the top-right corner. Enter the email address of your service account (it ends with @<your-project-id>.iam.gserviceaccount.com) and send the invite.

For using the tool you need to address:
1. name of file, for example "EventLog"
2. the address of EventLog.xlsx in your hadrd (if you load it locally) or the address of the downloaded JSON file (if you want to load the file from google drive)

It is recomended the testing and familiarity with the tool, chose the first approach.

**Step2** Download Neo4j Desktop

Download Neo4j-desktop-1.5.9

For downloading, first go to https://neo4j.com/download/
click download, then fill the form. Then clock on download desktop.
copy the code in order to install to activate your copy of Neo4j Desktop for use.


**Step3** Create a project and Local DBMS

Click on Add, then click on "Local DBMS", chose the a name anything that you want, then chose the password as "12345678", finaly chose the version of 5.17.0, and Then click on create
Then select the project, go to Plugins tab and install , select APOC and then click on Install. and finally click on Start.





**Step4** Install Chromedriver
Since is part of the project automated web tests using Selenium WebDriver with Google Chrome is used, it needed to install Chromedriver. First install the chrome browser (if not ) then 
We need to check our Google Chrome version: Open Google Chrome, go to Settings -> "About Chrome# to see our version. It's important that the ChromeDriver version matches the version of Chrome.
Then Download correct chromeDriver from (https://googlechromelabs.github.io/chrome-for-testing/) or (https://chromedriver.chromium.org/downloads). 
Unzip the downloaded file. Open the unzipped directory with terminal. Move it to a  user/bin  (sudo mv chromedriver /usr/bin/). the we set the exutable permission (sudo chmod +x /usr/bin/chromedriver). then verify the installation (chromedriver --version)



**Step5** Download the tool
Download the tool from application directory of the GitHub and install it and use it. There are three versions of the tools for three operating systems
Ubuntu:
Windows:
MacOS: 
