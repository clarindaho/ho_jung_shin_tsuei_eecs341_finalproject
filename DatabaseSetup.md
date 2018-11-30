## EECS 341 Project
Clarinda Ho (cqh), Seohyun Jung (sxj393), Jason Shin (jjs270), Catherine Tsuei (cwt26)

### Database Setup

#### Manual Setup
1. Install virtual environment by running
	<br> ***sudo apt-get install virtualenv***
2. Create virtual environment named eaterank
	<br> ***virtualenv eaterank***
3. Activate virtual environment
	- ***cd eaterank***
	- ***source bin/activate***
4. Install flask on virtual environment
	<br> ***pip3 install flask***
5. Install mysql connector
	<br> ***pip3 install mysql-connector***
6. Install supporting libraries
	- ***pip3 install requests***
	- ***pip3 install logger***
	- ***pip3 install configparser***
	- ***pip3 install bs4***
7. Create database on local machine
	- ***mysql -u root -p***
	- Enter mySQL password for **'root'**
	- ***SOURCE setup.sql;***
	- ***quit;***
8. To deactivate virtual environment
	<br> ***deactivate***

#### Automatic Setup
1. Make shell script executable
	<br> ***chmod +x setup.sh***
2. Run the shell script executable
	<br> ***./setup.sh***
3. Enter mySQL password for **'root'** when prompted

### Potential Error Solutions
- **'no module named configparser':**
	- ***pip3 install configparser***
- **'caching sha_2_password cannot be loaded':**
	- If using MySQL on Windows, set the user authentication method to **standard**