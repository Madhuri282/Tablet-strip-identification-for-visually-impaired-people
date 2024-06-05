# Tablet-strip-identification-for-visually-impaired-people
## Intoduction: 
The project aims to develop an innovative assistive technology solution that empowers visually impaired individuals to independently and accurately identify medicine strips.


![image](https://github.com/Madhuri282/Tablet-strip-identification-for-visually-impaired-people/assets/112135970/32d66408-0b17-4976-9b78-9a0f20b299f1)


## project set up guidelines:


SQL SETUP:

download mysql
create a password 

______________________________________________________________________________

QUERIES TO EXECUTE IN MYSQL COMMAND LINE CLIENT:

1)  create database medovision

2)  use medovision

3)  CREATE TABLE user (
        id INT AUTO_INCREMENT PRIMARY KEY,
        username VARCHAR(255) NOT NULL,
        phone_number VARCHAR(255) NOT NULL,
        password VARCHAR(255) NOT NULL
    );

4)  CREATE TABLE tablet_history (
        id INT AUTO_INCREMENT PRIMARY KEY,
        image_path VARCHAR(255) NOT NULL,
        identified VARCHAR(255),
        identified_tablet_name VARCHAR(255),
        similarity_score INT
    );

5)  CREATE TABLE daily_usage (
        id INT AUTO_INCREMENT PRIMARY KEY,
        tablet_name VARCHAR(255) NOT NULL,
        dosage VARCHAR(50) NOT NULL,
        frequency VARCHAR(20) NOT NULL
    );
_______________________________________________________________________________

PROJECT FOLDER SET UP:

download folder and open in vscode 

in sqlconnection.py file:
change host , user, password , database 
(host=localhost and user = root is usually by default)

________________________________________________________________________________


TO RUN

on vscode terminal run command:

>> streamlit run dashboard.py


_________________________________________________________________________________

note:
signup and login audio inputs need your microphone access so ensure it is on in your system settings and avoid bg disturbance while speaking.
