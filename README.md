# ContosoSite

Getting Started with Entity Framework 6 Database First Using MVC 5

https://learn.microsoft.com/en-us/aspnet/mvc/overview/getting-started/database-first-development/

<br><br>For reference only:
<br>These are steps to remove a file from repository commit history using <a href="https://rtyley.github.io/bfg-repo-cleaner">BFG Repo-Cleaner</a>. In this example the file name is Web.Somee.config (note possible case sensitivity):
<br>1. Delete Web.Somee.config from https://github.com/sharom01/contoso-university
<br>2. On the local pc add a new empty folder eg C:\Users\Sharom\source\repos\ContosoClone
<br> 3. In git bash:
```
$ cd "C:\Users\Sharom\source\repos\ContosoClone"
```
```
$ git clone --mirror https://github.com/sharom01/contoso-university.git
```
```
$ java -jar c:/bfg/bfg-1.14.0.jar --delete-files {Web.Somee.config}  contoso-university.git
```
```
$ cd contoso-university.git
```
```
$ git reflog expire --expire=now --all && git gc --prune=now --aggressive
```
```
$ git push
```
