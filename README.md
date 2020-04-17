# odoo-auto-deploy

steps to run build
---
Fill all the values in [properties file](build.properties) according to server configurations.

Setup GIT account and branch

Create boot script (./odoo-bin as service)

Install `ant`, `ant-contrib` and `jenkins`

Change **jenkins** user to **root** user

    Make change in file /etc/default/jenkins
    $JENKINS_USER = "root"
    
Change ownership of following files to `root:root`

    /var/chache/jenkins
    /var/lib/jenkins
    /var/log/jenkins
    
Give **root** permissions to **odoo directory** for storing **backups** and taking **git pull**





