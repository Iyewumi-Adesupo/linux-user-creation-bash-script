<h1 align="center" id="title">linux-user-creation-bash-script</h1>
                                                   <h1 align="center" id="title">User Management Bash Script</h1>

An Ubuntu machine on AWS is launched and connected. See below:

<img width="952" alt="launching an ubuntu machine ec2 instance" src="https://github.com/Iyewumi-Adesupo/linux-user-creation-bash-script/assets/135404420/665df9f1-e09b-4ddc-8b4b-46c4a5b33f8a">


<p id="description"> This repository contains a Bash script named create_users.sh designed to automate the process of creating users and assigning them to groups on a Linux system. The script reads a text file with usernames and group names, creates users, assigns them to the appropriate groups, generates random passwords, and logs all actions.

**Script Overview**
The create_users.sh script performs the following tasks:

<img width="947" alt="2 create a bash script  file" src="https://github.com/Iyewumi-Adesupo/linux-user-creation-bash-script/assets/135404420/8cdf8d0e-f27b-4dbe-a203-652a86f37bd8">




Reads a text file containing usernames and groups.
Creates users with their respective home directories.
Assigns users to specified groups.

<img width="950" alt="home directories fr users" src="https://github.com/Iyewumi-Adesupo/linux-user-creation-bash-script/assets/135404420/438bd571-e6b7-4d74-b7e2-7b9869131ff7">


Generates random passwords for the users.

<img width="947" alt="random passwrd" src="https://github.com/Iyewumi-Adesupo/linux-user-creation-bash-script/assets/135404420/3794b3b1-0a6e-4d5c-8140-20924ea36fac">

Logs all actions to /var/log/user_management.log.

<img width="947" alt="var management log" src="https://github.com/Iyewumi-Adesupo/linux-user-creation-bash-script/assets/135404420/3940016f-2263-4c40-80b0-3349c33e6776">


Stores the generated passwords securely in /var/secure/user_passwords.csv.

<img width="947" alt="random passwrd" src="https://github.com/Iyewumi-Adesupo/linux-user-creation-bash-script/assets/135404420/9151efe2-f3a2-4ead-a21f-1ba0f33ee6dd">


Usage
Prerequisites
The script must be run as root.
Ensure the necessary directories (/var/log and /var/secure) exist or will be created by the script.
Running the Script
To run the script, use the following command:

<img width="953" alt="end of script" src="https://github.com/Iyewumi-Adesupo/linux-user-creation-bash-script/assets/135404420/40eed69a-2ec3-484c-b83f-1f7f853df012">


The text file should contain lines formatted as user;groups, where user is the username and groups are the groups the user should belong to, separated by commas. Example:


On the terminal, cat the **userdata.txt** file consist of:
light; sudo,dev,www-data

idimma; sudo

mayowa; dev,www-data

<img width="946" alt="4 create userdata text for the usergroups" src="https://github.com/Iyewumi-Adesupo/linux-user-creation-bash-script/assets/135404420/612b9466-aeb0-4691-bdd2-b1057828e081">


<img width="948" alt="cat userdata" src="https://github.com/Iyewumi-Adesupo/linux-user-creation-bash-script/assets/135404420/d138f83e-fda2-49b9-be09-f6e0eef4638f">

