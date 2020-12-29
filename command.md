all the install package of the linux 
 	
	dpkg --list 



To uninstall a program, use the “apt-get” command, which is the general command for installing programs and manipulating installed programs. For example, the following command uninstalls git and deletes all the configuration files, using the “--purge” (there are two dashes before “purge”) command.

	sudo apt-get --purge remove git

If you don’t want to remove the configuration files, simply leave out the “--purge” command, as shown in the following command.
	
	sudo apt-get remove git

Programs installed in Linux depend on other packages to function. When you uninstall a program, there may be packages that the uninstalled program depended upon that are no longer used. To remove any unused packages, use the “autoremove” command, as shown in the following command.

	sudo apt-get autoremove 

You can combine the two commands for removing a program and removing dependencies that are no longer being used into one, as shown below (again, two dashes before “auto-remove”).

	sudo apt-get purge --auto-remove git

If you’re short on space, you can use the “clean” command to remove downloaded archive files, as shown below.

	sudo apt-get clean

NOte :
The “apt-get” is a handy tool that makes downloading, installing, and uninstalling programs quick and easy



To Install git on ubuntu 

	sudo apt-get install git


To check the git version

	git --version

To create a folder as a local git repository 

	git init 

To clone the remove repository 

    git clone url 

To check the status of the repository 

    git status

To track / add a file to staging area 

    git add file-name

To track / add all the modifing files to statuging area 

    git add . 
    git add -A

To untrack / or remove a file to the staging area 

    git rm --cached file-name  
    git rm -f --cached file-name

Records or snapshort the file permanently in the version control history 

    git commit -m "write a usefull commit here"

To find the latest commit 

    git show --summary
    git log .
    git log --oneline
    git log --oneline --graph ( to show graph)
    cat .git/refs/heads/branchName

To find the lastest head 

    git reflog

To Compare the version of the files

    git diff

To check the configuration of Remote repository 

    git config --local --list   ( for local )
    git config --global --list   ( for gobal )
    git config --list  ( for both )

To Configuring Git 
    git config --global user.name "username"
    git config --global user.email "useremail"

To set the remote repository 

    git remote add origin url

To Push the remote repository 

    git push -u origin master
    
To check the remove repository 

    git remote -v




    















