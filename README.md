# Git Basic Walkthrough

In this tutorial we will get a tree in git, with several branches intergrating with each other for a project. The following diagram will be our tree visualized  

## 1. Installation of Git
**a. search on google for Git's website**  
You can just click on this [link](https://git-scm.com/)👈.  

![Git's website on google](imgs/searchGit.jpg)  
<br>
<br>

**b. recon for Git's homepage**  
When locating the right web, this is what you will see in the first page.
![Git's homepage](imgs/gitHomePage.jpg)  

<br>
<br>

**c. Download page for Git**
Choose your preference based on your local system OS.
![Git's download page](imgs/gitDownloadPage.jpg)

<br>
<br>

**d. Installation for Git**  
Open the downloaded file from Git's web and follow the installation given, normally you just want to say yes to everything the installation recommends.
![Git installation app](imgs/gitInstallPage.jpeg)

<br>
<br>

**e. Verify your installation**
Type on `git --version`, and the output will be like this👇.  
![Git's version check](imgs/gitVersion.jpg)

<br>
<br>

**f. Make yourself an account**  
Type on `git config --global user.name "your name"` to add your name. Then don't forget to type on `git config --global user.email "your email"` to add your email, remember always use ` " " `.

<br>
<br>

**🎉Congratulation, you've done it, you installed Git🎊**  
Next step we will start using git to a project.


<br>
<br>

## 2. Start Growing Our Tree🌳
**a. First step**
Start with creating a folder anywhere you want your project to be, or an existing project is fine. Though in this walk through we will use empty folder
![Empty folder](imgs/emptyFolder.png)

<br>
<br>

**b. Set up**  
Open cmd in your folder, there are 2 ways, first right click on the empty folder and open cmd, or open cmd as usual but then you will need to do `cd` to your folder location.  

<br>

Then type on `git init` to initialize the Git system in your project folder.  
![Git terminal](imgs/gitInitTerminal.png)

 <br>
 <br>

**c. Creation**  
Now, after being initialized, we can start placing items in our folder. In this tutorial we will place simple txt files only, but the system and logic applies to greater scaled projects.
![Text files](imgs/textFiles.png)

 <br>
 <br>

**d. Adding**  
After having bunch of files aroun the folder, now we will add some files to the saving stage. By typing `git add` we will be able specifically move the file to the stage. In this walkthrough we will just add the `file1.txt` and `file2.txt` to the stage. Use `git add file1.txt` to just add that file, do the same for `file2.txt`.  
![Adding files](/imgs/gitAdd.png)

 <br>
 <br>

**e. Recon**  
We might lost track in the future about what files have we placed and what phase are we on, but don't worry too much. Git has a feature of `git status` to get information where you are right now and what has happened.  
![Git status](imgs/gitStatus.png)

 <br>
 <br>

**f. Commit**  
After adding them to the stage, saving in git is called as commit. `git commit -m "message"` will help you save and place a message, the message can be used to inform user what that save contain.  
![Git commit](imgs/gitCommit.png)

 <br>
 <br>

**g. Logs**  
In the future, there might be big changes given to your project, and not always a good change. When that happen, we always can revert to our old phase as long as we remember to save our progress. We can use `git log` to check on which changes we want to revert first.
![Git log](imgs/gitLog.png)

 <br>
 <br>

**h. Back in time**  
Alright, we have seen the log, just in case getting stuck on log, you can press `q` to exit. Back to seeing the log, we have seen the yellow text that looks like some hash codes, those codes will help us tell which save we want to revert to, in my example it's `a055cc2944975c43a481dbcc15d8310118b7832d`, now applying it to `git checkout` it will turn into `git checkout a055cc2944975c43a481dbcc15d8310118b7832d`, the output should look like this👇.  
![Git checkout](imgs/gitCheckout.png)

 <br>
 <br>

**i. Check your branch**
Now the next useful feature in Git is branch. Branch is like having the same print of homework with your friend.
You might want to do the homework differently from your friend, but the task given is the same. Branching is having the same file at any point you would like, and not to disturb other's progress, you can instead just duplicate it and start your own modifications  
![Git branch](imgs/gitBranch.png)