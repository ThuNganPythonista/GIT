# BASIC GIT COMMANDS AND SOME ERRORS GOOGLE OR CHATGPT NEVER DISCLOSE =)) #

*Git is Distributed Version Control System. It allows us to store changed versions of the project and go back to any version that has been saved. This system can be used by many people to work together on the same source code. And each person will have their own version of the source code. These separate versions can then be merged into the main version of the project.*

* It'll be easier when you already learnt Linux

### SECTION 1: INSTALL GIT AND RUN SOME BASIC COMMANDS TO PUSH YOUR PROJECT TO GITHUB ###

Firstly, you need to install GIT in your computer ! 

Install here : https://git-scm.com

![install git](./images/install-git.png)


Next, we will check whether it was installed or not.
You open cmd on Window or terminal on MacOs to check by the code `git --version`:

If it was like this, you did correctly :

![install git](./images/git.png)

### BASIC GIT COMMANDS ###

I can use Terminal in Visual Code Studio to code If you do not remember `Linux commands`

`git init`  : initialize a git repository local right in your folder

![install git](./images/git1-1.png)

 Now, you ALREADY CREATED a file `.git`  your folder
The file `.git` has been indicated in your project

`git add .` : it means like the meaning in English "add". You wanna anything, any files by using this commands. In this case, I use `.` meaning that add ALL. The format is `git add <file name>`. By the way, you can exclude any files by using `.gitignore`. I will tell you clearly later in this tutorial

![install git](./images/git1-1.png)


Okay !! There is one more step after `git add`.

You must commit changes by : `git commit -m “<any-contents-here>” `

Take note double quotation mark required, for example : `git commit -m “first commit”`

### *Take note :*  ###
Coppy code and paste can cause error due to double quotation marks, so you should type double quotation mark by yourself better.

![install git](./images/git2.png)

Done If your output exactly looks the same as mine !!! 

Now, you can check to be sure. Check commit : `git log`

![install git](./images/git3.png)

Here, it will display the commit ID (automatically generated by Git, which may be needed later), the commit author, commit time, and commit message.

Ta da! So, it's been saved. Now, let's move on to the next part, which is uploading the code to GitHub.

## *Let's Upload The Code to GitHub* # 

- Firstly, you should sign in GitHub Account : https://github.com/ . Please sign up If you don't have

- Secondly, click the button `New` after logged in :

![install git](./images/git4.png)

- Thirdly, After clicked, you will see this interface :

![install git](./images/git5.png)

Now, fill in necessary information :

 + Repository name : You name for your repo
 + Description : you describe your repo
 + Public or Private : Everyone will see your repo (public) or won't see (private)
 + Initialize files : README.md, .gitignore, license

Click "create repository" and then will see the next interface :

![install git](./images/git6.png)

Here, you see two instructions : create repo on the top and push an existing repo. Because we already created repo, we can ignore the first one. The second one is guidelines to push your local project to GitHub

- Now, you continue to code at your terminal, followed by 3 guidelines below. You just need to coppy and paste sequentially. For example, mine :
 
    `git remote add origin https://github.com/ThuNganPythonista/TEST.git`

  and then .. :

    `git push -u origin main`

  The output looks like this :

  ![install git](./images/git7.png)

  Now, your complete project is available on your repo GitHub already !!

### SECTION 2: Clone and Run a Django Project from Github ###

(1)Git clone : you create a coppy of the project on Github. You clone it into your local desktop, for example.

`git clone <URL of repo> `

(2)


### SOME COMMON GIT ERRORS
  
  ###### Message 'src refspec master does not match any'

  This error has two cases :
   + (1) No commit on master branch
   + (2) the name of local branch which is different from remote branch

  Debug :

  1. Check the status of master branch :
 
     `git status`

  2. If the output on terminal result like this :
 
     ![image]( https://github.com/ThuNganPythonista/GIT/blob/main/images/Screenshot%202023-12-01%20at%202.55.20%20PM.png)


 => Ya sure, your branch has no commit ! It means that you do not upload anything to your repo Github.

 But why you already run `git add .` ?

 The secret that Google and ChatGPT never tell you is hidden in `gitignore` file.

 Some project automatically created `gitignore` file, having (*) that means ignore EVERYTHING. Just delete it and run commands as usual, It will work !!!

 With MacOs, you must go to your finder and locate your project, run `command` + `shift` + `.` to show hidden git file.

 








