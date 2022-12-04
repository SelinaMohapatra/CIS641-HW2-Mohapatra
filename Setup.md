# Project Setup Instructions
## Clone the Backend Code
- From a terminal window clone the backend sourcecode from  https://github.com/manchint/GVSU-CIS641-sunrisers_base/tree/master/src/backend/cookbook

## Install Spring Tool suite(STS)
- Download Spring Tool Suite from https://spring.io/tools3/sts/all. Click on the platform which you are using.
- Extract the file and install the STS.
- Spring Tool Suite 4 Launcher dialog box appears on the screen. Click on the Launch button. You can change the Workspace if you want.
- STS is launched.
- Import the cloned project as Maven project.

## Install MySQL
- Download MySQL from https://dev.mysql.com/downloads/mysql/
- Extract the file and install the MySQL.
- Go to System Preferences and click on MySQL to check the server is running or not and check the configurations for the path set.
- From the terminal access the database by login in through the path specified in the configuration. eg:/usr/local/mysql/bin/mysql -u root -p
- Create a database using the following command: CREATE DATABASE <DATABASE_NAME>;



Create a dummy folder for sql backend for logging purpose
Open src/main/resources application.properties
Replace your SQL configuration

Right click on Project and Run as Spring Boot App
Then all the API’s should be appearing on this URL
http://localhost:8081/swagger-ui/index.html



