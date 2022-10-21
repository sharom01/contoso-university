# ContosoSite

Getting Started with Entity Framework 6 Database First Using MVC 5

https://learn.microsoft.com/en-us/aspnet/mvc/overview/getting-started/database-first-development/

<br><br><br>For reference only:
<br>Removing a file from repository commit history using <a href="https://rtyley.github.io/bfg-repo-cleaner">BFG Repo-Cleaner</a> 
<br>In this example the file name is Web.Somee.config (possibly case sensitive)
<br>Steps:
<br>Delete Web.Somee.config from https://github.com/sharom01/contoso-university
<br>On the local pc add a new empty folder. Here it is C:\Users\Sharom\source\repos\ContosoClone
<br>In git bash:
<br>cd "C:\Users\Sharom\source\repos\ContosoClone"
<br>git clone --mirror https://github.com/sharom01/contoso-university.git
<br>java -jar c:/bfg/bfg-1.14.0.jar --delete-files {Web.Somee.config}  contoso-university.git
<br>cd contoso-university.git
<br>git reflog expire --expire=now --all && git gc --prune=now --aggressive
<br>git push
