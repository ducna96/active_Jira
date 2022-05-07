
########### Install JDK/JRE ###########
[Windown]
download Jdk in http://www.oracle.com/technetwork/java/javase/downloads/index.html
Version suggest: 1.8 (>=1.7)

[Linux->Ubuntu 16.04]
sudo apt-get update
sudo apt-get install oracle-java8-installer

######### Install Mysql >=5.7 ##########
[Windown]
download: https://dev.mysql.com/downloads/mysql/
Version suggest: MySQL Community Server 5.7.*

[Linux->Ubuntu 16.04]
sudo apt-get update
sudo apt-get install apache2
sudo apt-get install mysql-server libapache2-mod-auth-mysql php5-mysql
sudo apt-get install php5 libapache2-mod-php5 php5-mcrypt

########## Import data to DB ###########
CREATE DATABASE jira CHARACTER SET utf8;

GRANT ALL PRIVILEGES ON jira.* TO jira@127.0.0.1 identified by 'Nguyenkien.2793';
GRANT ALL PRIVILEGES ON jira.* TO jira@172.18.31.240 identified by 'Nguyenkien.2793';
GRANT ALL PRIVILEGES ON jira.* TO jira@lab1 identified by 'Nguyenkien.2793';
FLUSH PRIVILEGES;

NOTE: 172.18.31.240 is ip server 

############# Install Jira #############
Version latest: 7.7.0

download: 
In website Jira: https://www.atlassian.com/software/jira/download

linux x64: https://www.atlassian.com/software/jira/downloads/binary/atlassian-jira-6.4.14-x64.bin
linux x32: https://www.atlassian.com/software/jira/downloads/binary/atlassian-jira-6.4.14-x32.bin
Tar.gz: https://www.atlassian.com/software/jira/downloads/binary/atlassian-jira-6.4.14.tar.gz
Windown x32: https://www.atlassian.com/software/jira/downloads/binary/atlassian-jira-6.4.14-x32.exe
Windown x64: https://www.atlassian.com/software/jira/downloads/binary/atlassian-jira-6.4.14-x64.exe
Zip: https://www.atlassian.com/software/jira/downloads/binary/atlassian-jira-6.4.14.zip

OR: https://drive.google.com/drive/folders/12y7A4HpYFsWQ-T1Gn77rSGA6BMRO5btz?usp=sharing
Download JIRA APPLICATION

[Windown]
Installing

[Linux->Ubuntu 16.04]
chmod a+x atlassian-jira-software-7.5.0-x64.bin 
./atlassian-jira-software-7.5.0-x64.bin 

########## Add MySQL connector ##########
download: wget http://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-5.1.30.tar.gz

OR: https://drive.google.com/drive/folders/12y7A4HpYFsWQ-T1Gn77rSGA6BMRO5btz?usp=sharing
Download: mysql-connector-java-5.1.38-SNAPSHOT-bin.jar
UnZip if Zip File

[Windown]
Copy to jira_home/atlassian/jira/lib/

[Linux->Ubuntu 16.04]
tar -xvzf mysql-connector-java-5.1.30.tar.gz
cp -r mysql-connector-java-5.1.30/mysql-connector-java-5.1.30-bin.jar ~/atlassian/jira/lib/

################# Active ################
https://drive.google.com/drive/folders/12y7A4HpYFsWQ-T1Gn77rSGA6BMRO5btz?usp=sharing

Download: "Crack Jira All Version [NoBiTa-KN].zip"
Unzip if Zip File

$$$$ stop jira $$$$

--------------------
[Windown]
start keygen.bat

[Linux->Ubuntu 16.04]
bash keygen.sh
---------------------

[Patch Extras] to atlassian-extras-x.x.x.jar file. 
Link: ~/atlassian/jira/atlassian-jira/WEB-INF/lib/atlassian-extras-x.x.x.jar

[Patch Plugin] to atlassian-universal-plugin-manager-plugin-x.x.x.jar file. 
Link: ~/atlassian/jira/atlassian-jira/WEB-INF/atlassian-bundled-plugins/atlassian-universal-plugin-manager-plugin-x.x.x.jar

$$$$ start jira $$$$

[Generate] 
Fill all info (Contact Name, Contact Email, Organisation, Server ID)
Example: 
Contact Name: Kien Nguyen
Contact Email: nguyenkien25@nobita.kn
Organisation: NoBiTa-KN
Server ID: BC28-W78S-9GH1-E4RG

Click [Generate] => Copy key in "Generate Key" to License key Jira

####### NOTE: Search Server ID & Licenses in Jira ########
[Jira >= 7.0]
Licenses Key: Setting Administration => Applications => Versions & licenses
Server ID   : Setting Administration => System => Server Info => Server ID

[Jira < 7.0]
Licenses Key & Server ID: Setting Administration => System => License

====================================NôBiTa-KN====================================