Create an Ansible playbook that targets members of the "app" group has the following state:The tomcat7 is installed in all host
Has the war file in webapps folder specified in appwar.
Tomcat is started on each host.

We have created tomcat role

![](Aspose.Words.7f9798de-a8e2-430d-8415-b92feb0d60c6.001.png) 

We have inventory file as

![](Aspose.Words.7f9798de-a8e2-430d-8415-b92feb0d60c6.002.png) 

Execution of Playbook

![](Aspose.Words.7f9798de-a8e2-430d-8415-b92feb0d60c6.003.png)



![](Aspose.Words.7f9798de-a8e2-430d-8415-b92feb0d60c6.004.png) 

After Executing our tomcat are up and running with war file

![](Aspose.Words.7f9798de-a8e2-430d-8415-b92feb0d60c6.005.png) 

![](Aspose.Words.7f9798de-a8e2-430d-8415-b92feb0d60c6.006.png) 

While developing the playbook use the --syntax-check to check your work and debug problems. Run your playbook in verbose mode using the -v switch to get more information on what Ansible is doing. Try -vv and -vvv for added verbosity. Also consider running --check to do a dry-run as you are developing.

![](Aspose.Words.7f9798de-a8e2-430d-8415-b92feb0d60c6.007.png) 

![](Aspose.Words.7f9798de-a8e2-430d-8415-b92feb0d60c6.008.png) 

![](Aspose.Words.7f9798de-a8e2-430d-8415-b92feb0d60c6.009.png)
