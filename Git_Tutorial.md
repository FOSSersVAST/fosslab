# Version Control System using Git

#### What is Git?

-----

**Git** is  a distributed version-control system for tracking changes in source code during software development. 

Git was created by _Linus Torvalds_ in 2005 for development of the Linux kernel, with other kernel developers contributing to its initial development. Its current maintainer since 2005 is _Junio Hamano_. 

Git is free and open-source software distributed under the terms of the GNU General Public License version 2.



#### Setting up the system

------

Before going to use git we want  to check whether your system has [git](https://git-scm.com/).

For checking whether you have git type the following,

```bash
$ git --version
```

For installing git in your system

```bash
$ sudo apt-get install git
```

Then open up the terminal and update your git account.

```bash
$ git config --global user.email "username@example.com"

$ git config --global user.name "Your Name"
```

For clone a git repository use,

```bash
$ git clone https://github.com/....
```

#### Basic git commands

------

For checking the status of your edit,

```bash
$ git status
```



For adding your edit to the origin/master branch,

```bash
$ git add .
```



For committing your edit to the master branch,

```bash
$ git commit -m "Some random message"
```



For pushing your code to remote server,

```bash
$ git push
```



If you got conflict error the update the git repository by,

```bash
$ git pull
```

and call 

```bash
$ git mergetool
```

for fixing the conflict.

Use the default conflict resolver ``meld`` for graphical conflict resolving.

## Exercise

Here were are going to do some action in Github.

The main steps in done in this program

1. Fork the repository
2. Edit the content
3. Commit your edits
4. Push your edits
5. Create Pull Request (**PR**)

#### 1. Fork the repository

------

First fork the repository from the source  by clicking on the fork button on the right-most part of the repository.

Now you have got a duplicate/fork of the repository.

Now we need to save our repository to our local system or computer. We need to copy the URL of your repository and do following command.

```bash
$ git clone https://github.com/examplerepo
```

Now we have successfully saved the repository to your system.

#### 2. Editing

------

Edit your files by using text editors like gedit, sublimetext,etc.

#### 3. Committing

----

**Note : ** Before this you should be in the root of the local clone of the repo.

It is recommended to commit every edits you do as it will easier for you to return to previous code. So for committing your edits do the below code.

```bash
$ git add .
$ git commit -m "Edited file!!"
```

#### 3. Push

------

After editing your file, we now have to update your repository in the remote server ,i.e in Github's server. For this we use ``push`` command.

```bash
$ git push
```

After this , we have successfully updated the repository in the server.

Note : At this stage you may have encountered an error due to mail privacy. To solve this just uncheck the Email privacy in the Email Tab in your Profile Settings. For more info regarding this error, click here.

#### 4. Create Pull Requests

Now we have reached to the last and important stage of our session. Creating  pull request is basically adding your new features to the master branch of the repository.

To create **PR**, click on 'New Pull Request' in th 'Pull Request' Tab in your repository. Then compare both of your edits and apply for **PR**. Now a dialog box will come and add some details. Then click submit.

Now you have made your Pull Request or simply your **PR** !!

#### 5. Pulling from Upstream

Upstream refers to the main repository from where you forked. You need to mention the URL of the main repo to pull changes from it :

```bash
git remote add upstream https://github.com/example/examplerepo.git
```

Now you can pull changes from the `master` branch of the main repository :
```bash
git pull upstream master
```
