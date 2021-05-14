Create and delete ninja directory on host machine

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.001.png)

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.002.png) 

Set hostname on all nodes from remote machine

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.003.png) 

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.004.png) 

Fetch os of all nodes and store o/p into a file, use min two different machine of different flavour of os.



![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.005.png) 

Add three group into hosts file through ansible module.

We made a playbook block.yml for achieving this and a blank hosts file named hosts\_new.

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.006.png) 

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.007.png) 

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.008.png) 

Using Adhoc Commands

Install apache on Debian machine



![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.009.png) 

Cross check apache isntalled or not from remote machine

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.010.png) 

Apache running  on 8082 port

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.011.png)



![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.012.png) 

Create two virtual host and Restart apache from remote machine

We will copy 2 directory in /var/www with index.html and 2 conf files in /etc/apache2/sites-available and then create 2 symlink at /etc/apache2/sites-enabled

Copy Site 1

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.013.png) 

Copy Site 2

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.014.png) 

Copy Conf file for site 1

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.015.png) 

Copy Conf file for site 2

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.016.png) 

Creating Soft link

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.017.png) 

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.018.png) 

Making entry of port 8083 and 8084 in ports.conf

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.019.png) 

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.020.png) 



![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.021.png) 

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.022.png) 

Install nginx on centos machine

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.023.png)

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.024.png)  

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.025.png)

Nginx run on 8080 port and Configure Nginx - configure it to run as reverse proxy to apache

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.026.png) 

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.027.png) 

For SELinux Permission issue

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.028.png) 

![](Aspose.Words.298b79a0-14e4-41c3-83a1-83d962a26da8.029.png)
