install and crack jira all version
#download jira from docker
https://github.com/ducna96/docker_Jira
#dowload tool
https://drive.google.com/drive/folders/12y7A4HpYFsWQ-T1Gn77rSGA6BMRO5btz
#connect docker container of jira to copy 2 file need patch atlassian-extras-3.2.jar,atlassian-universal-plugin-manager-plugin-2.22.9.jar
docker exec -it dockerjira_jira_1 bash
cd  opt/jira/atlassian-jira/WEB-INF/lib/
#creat file backup 
mv atlassian-extras-3.2.jar atlassian-extras-3.2.jar.bak

cd /opt/jira/atlassian-jira/WEB-INF/atlassian-bundled-plugins
mv  atlassian-universal-plugin-manager-plugin-2.22.9.jar atlassian-universal-plugin-manager-plugin-2.22.9.jar.bak
exit

#copy 2 file need patch to server
docker cp dockerjira_jira_1:/opt/jira/atlassian-jira/WEB-INF/lib/atlassian-extras-3.2.jar.bak ./
docker cp  dockerjira_jira_1:/opt/jira/atlassian-jira/WEB-INF/atlassian-bundled-plugins/atlassian-universal-plugin-manager-plugin-2.22.9.jar.bak ./
#copy 2 file from server to window
#on window : 
scp root@ipserver:/root/docker-jira/atlassian-extras-3.2.jar.bak ./
scp root@ipserver:/root/docker-jira/atlassian-universal-plugin-manager-plugin-2.22.9.jar.bak ./
#[Generate] 
Fill all info (Contact Name, Contact Email, Organisation, Server ID)
Example: 
Contact Name: AnhDuc	
Contact Email: duc.na1006@gmail.com
Organisation: Vicoder
Server ID: BC28-W78S-9GH1-E4RG
Click [Generate] 
copy 2 file was patched to container of server and restart docker-compose
=> Copy key in "Generate Key" to License key Jira
