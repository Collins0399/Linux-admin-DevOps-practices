# Creating a Service User Without a Home Directory on App Server

### In response to the latest tool implementation at xFusionCorp Industries, the system admins require the creation of a service user account. Here are the specifics:

## Objective:
To comply with xFusionCorp Industries’ latest tool implementation requirements, Create a user named rose in App Server 1 without a home directory without generating a home directory, ensuring minimal resource usage and adhering to system admin policies.

## Steps to Add a User Without a Home Directory
### 1. Log in as root or a sudo user
```bash
ssh user@server
```
### 2. Use useradd with the -M option
```bash
sudo useradd -M rose
```
 #### -M means do not create a home directory.

### 3. (Optional) Set a password for the user
```b
sudo passwd rose
```
### 4. Confirm user was added without home
```bash
grep rose /etc/passwd
```
#### Output
```bash
rose:x:1002:1002::/home/rose:/bin/bash
```
#### Even though /home/rose is listed, the directory doesn't exist unless it was manually created.

### 5. Verify the directory doesn’t exist
```bash
ls -ld /home/rose
```
#### Output

##### ls: cannot access '/home/rose': No such file or directory

## Summary:
### a. Create user with no home 
#### sudo useradd -M rose
### b. Set password 
#### sudo passwd rose
### c. Confirm user creation 
#### grep rose /etc/passwd
### d. Check home dir absence
#### ls -ld /home/rose

![alt text](../assets/Task3.png)

