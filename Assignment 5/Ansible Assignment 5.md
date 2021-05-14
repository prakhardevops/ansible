All needs to be done using ansible modules with jenkins There will be three jenkins jobs, Provisioning, Build, Deployment.

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.001.png) 

Provisioning:-

` `Provision application servers, for example - java, tomcat are required for a java project.This job will be a separate job and can be executed to any machine on requirement.

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.002.png) 

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.003.png)


![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.004.png)

Build:-

Build any Project - can be java or any other language using jenkins.

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.005.png) 

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.006.png) 

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.007.png) 

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.008.png) 

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.009.png)

Deployment:-

Create a down stream deployment job to the build job .In the deployment job , deploy the artifact (war in case of java) to the application server (tomcat/joboss) using ansible in the downstream job. Ansible play book will include health check also, (status code == 200) , if health check fails, job should also fail.

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.010.png) 

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.011.png) 

For health check of url we have made mistake knowingly as passing wrong url for build failure




![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.012.png) 

We have right and wrong artifact name in vars file. We used right path is ubuntu.yml and wrong in redhat.yml

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.013.png) 

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.014.png)



![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.015.png) 

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.016.png) 

Build got failed as we were passing wrong url for redhat server.

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.017.png) 

![](Aspose.Words.f98f0bcb-8a54-4df1-b577-84d34cc3bd1b.018.png)
