# Linux_DevOps_commands
#!/bin/bash
##### Author : Pranab
##### Purpose : Usefull Linux command for DevOps 
##### Date : 14-May-24
############# Start of commands ##############
date
#date; sudo su -
#date ; su - 
date ; whoami
date ; cd ~
date ; cd /etc
date ; pwd
date ; ls -ltra
date ; touch /tmp/devops.log
date; cat > /tmp/devops1.log << eof
  " Hello , Welcome Devops world"
eof
mkdir -p /tmp/devops/
rmdir /tmp/devops/
mkdir -p /tmp/devops_v1/
cp -p /tmp/devops.log /tmp/devops_v1/.
mv /tmp/devops.log /tmp/devops_v1/.
tee -a /tmp/devops2.log << eof
"Shell scripting is an essential skill for DevOps engineers, as it empowers you to automate tasks, streamline processes"
eof
echo "
By using vi editor or vim editor we can create files with data \
vi filename \
vi pavani1 \
press i to insert the data \
to save the data :wq! \
to quit the saving data :q \
"
touch /tmp/devops.flag
ls -ltr /tmp/devops.flag
rm -rf /tmp/devops.flag
cat /etc/os-release | grep ubuntu
echo "less /etc/os-release"
echo "more /etc/os-release" 
head -n 5 /etc/os-release
tail -n 3 /etc/os-release
cat > /tmp/devops.cfg << eof
1
4
3
2
eof
cat /tmp/devops.cfg
sort /tmp/devops.cfg
echo "history"
cd /tmp
#wget https://nodejs.org/dist/v20.13.1/node-v20.13.1.tar.gz
#tar -xvzf /tmp/node-v20.13.1.tar.gz
cd -
yum -y install python
cd /tmp
wget https://rpmfind.net/linux/fedora/linux/development/rawhide/Everything/aarch64/os/Packages/m/mysql-8.0.36-3.fc40.aarch64.rpm
rpm  -ivh mysql-8.0.36-3.fc40.aarch64.rpm

du -sh
df -sh
free -mh
uptime

echo "
user
-->A person who uses the system to use services and resorces.
-->Creating user
useradd pavani
grep pavani /etc/passwwd
-->Assign password to user
passwd pavani
enter the password
grep pavani  /etc/shadow
group
-->A collection of users is called group
-->Creating group:
groupadd devops
-->Assign password
gpasswd devops
-->Adding users to group
gpasswd -M pavani devops
gpasswd -M username groupname)
"
cat /etc/os-release
wc -l /etc/os-release
find /etc -name os-releas
yum -y install httpd
systemctl status httpd
sudo apt -y install traceroute
traceroute google.com
ping -c 4 google.com
ifconfig all
sudo apt -y install net-tools
route
hostname
echo "sudo hostname <newname>"
