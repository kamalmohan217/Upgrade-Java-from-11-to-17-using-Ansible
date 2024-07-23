# Upgrade Java from 11 to 17 using Ansible

Provide 600 permission on private key  testkey.pem using the command **chmod 600 testkey.pem** 

![image](https://github.com/user-attachments/assets/21a17602-164a-4d77-b46e-9c64b6986562)

Command to run ansible-playbook is shown below
![image](https://github.com/user-attachments/assets/d7bd21d6-10a5-40a7-a41c-eb9453cca651)
<br><br/>
java version, JAVA_HOME and PATH before and after the Java Upgrade is shown in Screenshots below.

**Before Java Upgrade on Amazon Linux2**
![image](https://github.com/user-attachments/assets/51a0d159-bd97-4842-b61e-7e41edacf011)

**After Java Upgrade on Amazon Linux2**
![image](https://github.com/user-attachments/assets/12b118a0-ddce-4075-8f69-e2866cb6699d)

**Before Java Upgrade on Rocky Linux**
![image](https://github.com/user-attachments/assets/828051e5-4af5-4c60-b6bc-c873ebed8dc3)

**After Java Upgrade on Rocky Linux**
![image](https://github.com/user-attachments/assets/d902140d-c9bf-4bdf-9936-e29fd6dc5bb1)

**Before Java Upgrade on Alma Linux**
![image](https://github.com/user-attachments/assets/eae08a9d-ab16-4da9-82d6-36db82940593)

**After Java Upgrade on Alma Linux**
![image](https://github.com/user-attachments/assets/4a1dbf5c-f5d8-4078-9e14-e0d1a9f5e7d6)

**Before Java Upgrade on RHEL8**
![image](https://github.com/user-attachments/assets/eeeedec0-97ee-4fed-8f09-462942adf2ab)

**After Java Upgrade on RHEL8**
![image](https://github.com/user-attachments/assets/e50b42b9-4d38-4758-804e-159a9189c3c3)

![image](https://github.com/user-attachments/assets/9c523538-323d-4216-8752-d85c87b3b9f5)

**Before Java Upgrade on Ubuntu**
![image](https://github.com/user-attachments/assets/dc2d905b-5254-470c-91c9-c429fda371eb)

**After Java Upgrade on Ubuntu**
![image](https://github.com/user-attachments/assets/0d49f955-386b-47c0-b039-efc52ffa9daa)
<br><br/>
<br><br/>
<br><br/>
command to know the ansible_os_family, ansible_distribution etc.
```
ansible -i ./inventory/hosts -u ritesh --private-key testkey.pem -m setup | grep -i "ansible_os_family"
ansible 52.170.102.16 -i ./inventory/hosts -u ritesh --private-key testkey.pem -m setup | grep -i "ansible_distribution"
```
