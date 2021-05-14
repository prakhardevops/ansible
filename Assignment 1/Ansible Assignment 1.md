Use pip to install the ansible package and its dependencies to your control machine.

![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.001.png) 

![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.002.png) 

Display the Ansible version and man page to STDOUT.

![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.003.png)




![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.004.png) 

Check all the possible parameters you need to know in ansible.cfg file.

![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.005.png)

Ansible Inventory: Check the default inventory file for ansible control master and use inventory, run ansible ping commands on various inventory groups. Try this on minimum of two virtual machines.(You can use any of these Docker/Vagrant)

` `![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.006.png)

![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.007.png)  







5. In ~/.ansible.cfg file (create the file if it doesn't exist already) do the following:
- Create a new directory ~/.ansible/retry-files and set retry\_files\_save\_path to it.
- Set the Ansible system forks to 10

![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.008.png) 

![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.009.png) 

Host a static website on minimum three hosts using inventory, content of static website is "Index page of Ansible assignment"

Document root /opt/html

` `![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.010.png)

` `![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.011.png) 

` `![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.012.png) 

\- First do this manually and then with jenkins using ansible plugin or execute shell.

\- only use ansible modules.

![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.013.png) 

![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.014.png) 

![](Aspose.Words.5c28d892-dcb4-4390-ade7-5b7b50ad44f2.015.png)
