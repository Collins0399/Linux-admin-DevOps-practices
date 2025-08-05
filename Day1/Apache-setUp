## How to Set Up a Custom Apache User on a Linux Server with Specific UID and Home Directory
---

### Objective
Configure Apache (HTTPD) to run as a custom non-root user instead of the default user like www-data (Debian/Ubuntu) or apache (CentOS/RHEL).

### Procedure
---
#### 1️⃣ SSH into App Server 1
```bash
ssh tony@stapp01

```
---
#### 2️⃣ Create the User john with UID and Home Directory
```bash
sudo useradd -u 1091 -d /var/www/john -m john

```
```bash
# Assigns user ID
-u 1091: 

# Sets the home directory
-d /var/www/john: 

# Creates the home directory
-m: 
```
---

### Optional
#### Set a non-interactive shell:

```bash
sudo usermod -s /sbin/nologin john
```
---

#### 3️⃣ Verify the User
```bash
id john
grep john /etc/passwd
ls -ld /var/www/john

```

### Example output:
```bash
uid=1091(john) gid=1091(john) groups=1091(john)
john:x:1091:1091::/var/www/john:/sbin/nologin
drwxr-xr-x 2 john john 4096 Aug 5 12:00 /var/www/john

```
---
### Example

![My Screenshot](../assets/custom_apache_set_up.png)

---