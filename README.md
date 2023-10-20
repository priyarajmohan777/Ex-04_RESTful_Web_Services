# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.

Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.
![image](https://github.com/priyarajmohan777/Ex-04_RESTful_Web_Services/assets/119475942/af906bec-c4a7-4689-b3fe-bee14380d265)




Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 ![image](https://github.com/priyarajmohan777/Ex-04_RESTful_Web_Services/assets/119475942/dd6edfa1-10d4-47f1-9093-7325ded765e6)

 


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.
![image](https://github.com/priyarajmohan777/Ex-04_RESTful_Web_Services/assets/119475942/b574628c-be51-43fe-9fea-a653d35ec2a8)


Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
 
![image](https://github.com/priyarajmohan777/Ex-04_RESTful_Web_Services/assets/119475942/d290bb12-036d-4a8a-8710-2bef1c2f4e7c)

 


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.


![image](https://github.com/priyarajmohan777/Ex-04_RESTful_Web_Services/assets/119475942/5f804c1a-2214-4cd2-8f0a-bfd9544c8b05)


Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. 
Step 4: Carefully select your RESTful resource (web service) and click OK.
 
 ![image](https://github.com/priyarajmohan777/Ex-04_RESTful_Web_Services/assets/119475942/78eb4a65-f516-4990-87ba-d5cc1993c13a)



Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.
![image](https://github.com/priyarajmohan777/Ex-04_RESTful_Web_Services/assets/119475942/ab186321-7322-4ce1-976c-a25afef0c271)


Step 6: An editing tab will open. Alter getHtml() method with the following.
 ![image](https://github.com/priyarajmohan777/Ex-04_RESTful_Web_Services/assets/119475942/b13e6eac-44ed-4641-aa45-716210016472)

 

Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.
![image](https://github.com/priyarajmohan777/Ex-04_RESTful_Web_Services/assets/119475942/1b8bbed1-1cd7-4748-905e-6296d0aed6f3)


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 
![image](https://github.com/priyarajmohan777/Ex-04_RESTful_Web_Services/assets/119475942/d2364c60-bba0-4569-942f-0fb84dec90d7)
 


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.
![image](https://github.com/priyarajmohan777/Ex-04_RESTful_Web_Services/assets/119475942/54858d58-e0fd-411c-b595-97aa55652f43)


Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
 
 ![image](https://github.com/priyarajmohan777/Ex-04_RESTful_Web_Services/assets/119475942/87faad4f-8131-49a4-84b7-46a54f88e789)



Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
