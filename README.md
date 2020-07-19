# dev-basics

## Git Operations
Follow these steps if you have a an existing repo in GitHub to work on 
1. Cloning a remote source code repository
	
```bash
git clone your-example-repo-uri
```
2. Committing the changes made, it is a two step process - first you stage the chnages by runnning 
```bash
git add -A
```
then, you commit the staged changes by running 
```bash
git commit -m "your commiy message"
```
3. Now push your locally committed changes to the remote(also called origin) repository - In our case, we are using GitHub as our origin/remote	 
Things to be noted
	i) Never push directly to remote master branch
	ii) Always create a new branch locally and push to the same new remote branch, put a pull requests to Master in the remote, 
	   so that if there anyone else working on the same repo will be able to review the changes you made, and then merge it to master.


### Unix basics:
the symbol `~` represents user's (here it is you - vinitha) home directory :    `/Users/vinitha`
so in mac os, `~` is equal to users home dir path-  `/Users/<username>`

Lets say your terminal is at some where in your file system and you want to go to your home directory, then you can go by simply running the following command	
```bash
cd ~
```
assume you a directory called cfiles in your home directory, and you want to navigate to that directory 
```bash
cd ~/cfiles
```
Dangerous command in Unix, Should be used with caution
```bash	
rm        #this command can be used to delete files or directories
```

### Working with Go Projects in your computer:

1. Create a project directory 
```bash
  ~/go/src/github.com/<user-name>/<repo-name>
```

2. go to your project directory
```bash
cd ~/go/src/github.com/<user-name>/<repo-name>
```

3. Initialize your project as a go module - 
```bash
go mod init
```
4. Start coding 

5. Run you code by using - `go run` command - for example: 
```bash
go run ./main.go
```
