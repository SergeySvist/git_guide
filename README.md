# Git configs

After installing Git, you need to check the correct installation and version, for this you can use this command in console:

```properties 
git --version
```

Once you've made sure everything works well, you need to save your name and email in the configs:

```properties 
git config --global  [user.name](http://user.name/) "John Doe"
```
```properties 
git config --global [user.email](http://user.email) [johndoe@example.com](mailto:johndoe@example.com)
```

Command to view the list of configs:

```properties 
git config --list
```

# Git work with project

After setting up the configs and creating your project, you can start using Git.

To start using Git, type this command in your project folder:
```properties 
git init
```

You can check the status of your project files with this command (If the files are red, then they are not saved):
```properties 
git status
```

To create a save, you must first add files using these commands:
```properties 
git add main.cpp
```
```properties 
git add .
```

You can save the state of the project and make a commit using this command:

```properties 
git commit -m "my new commit"
```

These commands are needed to view the list of commits:
```properties 
git log
```
```properties 
git log --pretty=oneline
```

# Git work branches

Commands for creating a branch:
```properties 
git branch
```
```properties 
git branch dev
```

Command to go to the specified branch:

```properties 
git checkout dev
```

Command to delete a branch:
```properties 
git branch -D dev
```

Commands for merging branches:
```properties 
git checkout dev
```
```properties 
git merge fix
```

# VIW commands

This section shows the most useful commands in vim (and yes, they are all for exiting it)

`:wq`	write quit
`:q!`	quit without changes
`:q`	        quit

# Work with remote branch and GitHub

To start working with GitHub, you need to generate an ssh key:

```properties 
ssh-keygen -t rsa -b 4096 -C "[your_email@example.com](mailto:your_email@example.com)"
```

```properties 
cat id_rsa.pub
```

Add public key to GitHub

Add remote reference to your local repository:
```properties 
git remote add origin git@github.com:SergeySvist/Deadline.git
```

Push branch in GitHub:
```properties 
git push origin dev
```

View remote branches:
```properties 
git remote -v
```

Deleting remote branches:

```properties 
git remote rm origin
```
