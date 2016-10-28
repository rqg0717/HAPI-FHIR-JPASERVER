# HAPI-FHIR-JPASERVER
HAPI FHIR server running on Tomcat using MySQL database



Install Tomcat.

Make sure you have Tomcat set up in IntelliJ.
File->Settings->Build, Execution, Deployment->Application Servers
Click +
Select "Tomcat Server"
Enter the path to your tomcat deployment for both Tomcat Home

Add a Run Configuration for running hapi-fhir-jpaserver under Tomcat
Run->Edit Configurations
Click the green +
Select Tomcat Server, Local
Change the name to whatever you wish
Uncheck the "After launch" checkbox
On the "Deployment" tab, click the green +
Select "Artifact"
Select "hapi-fhir-jpaserver:war"
In "Application context" type /hapi

Run the configuration
You should now have an "Application Servers" in the list of windows at the bottom.
Click it.
Select your server, and click the green triangle (or the bug if you want to debug)
Wait for the console output to stop
