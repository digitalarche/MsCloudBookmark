
# For debugging WebApp Service

Kudu is not a security tool, but it is indeed very useful debugging tool.

For each Azure web app, which may contain a single function or more, 
there is a corresponding Kudu website to debug and manage the functions.
Kudu was developed by Microsoft and it allows debugging of both Windows and Linux based functions.

It is accessed by browsing ** https://*.scm.azurewebsites.net ** where the wildcard is your web app name.

With Kudu, you can download Docker logs, browse your home directory files (the shared directory), 
see your function Git endpoint and much more.
Kudu functionality varies between Windows and Linux environment, 
as the deployment and features of Azure Functions also varies when changing operating system.

Most of Kudu’s functionality is exported using REST API.


