Fetch and display to STDOUT Ansible facts using the setup module.

![](Aspose.Words.13248ea6-306c-411c-b681-9e75e3058372.001.png) 

Fetch and display only the "virtual" subset of facts for each host.

![](Aspose.Words.13248ea6-306c-411c-b681-9e75e3058372.002.png) 

Fetch and display the value of fully qualified domain name (FQDN) of each host from their Ansible facts.

![](Aspose.Words.13248ea6-306c-411c-b681-9e75e3058372.003.png) 

Display the uptime of all hosts using the command module.

![](Aspose.Words.13248ea6-306c-411c-b681-9e75e3058372.004.png) 

Ping all hosts except the 'control' host using the --limit option

![](Aspose.Words.13248ea6-306c-411c-b681-9e75e3058372.005.png) 

Setup Java8 on the hosts in the "App" group using the apt module.

![](Aspose.Words.13248ea6-306c-411c-b681-9e75e3058372.006.png) 

Setup and enable the EPEL package repository on the hosts in the "web" group using the yum module. CentOS systems use the latest epel-release package

RHEL systems should use <https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm>

![](Aspose.Words.13248ea6-306c-411c-b681-9e75e3058372.007.png)



![](Aspose.Words.13248ea6-306c-411c-b681-9e75e3058372.008.png) 

![](Aspose.Words.13248ea6-306c-411c-b681-9e75e3058372.009.png) 

set a cron on ansible control machine that will run every 1 minute ,  and perform below tasks:-execute ansible adhoc commands on client machines (cannot be control machine) , to  create a file in /var/log/ninja\_name on all the client nodes,

append system\_hostname [:space:] system\_time in the file every 1 minute using ansible facts.

![](Aspose.Words.13248ea6-306c-411c-b681-9e75e3058372.010.png) 



![](Aspose.Words.13248ea6-306c-411c-b681-9e75e3058372.011.png) 

![](Aspose.Words.13248ea6-306c-411c-b681-9e75e3058372.012.png)
