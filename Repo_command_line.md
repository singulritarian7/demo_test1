Creating Repository in GitHub
Objectives of this Exercise

To create a repository in GitHub with README.md
To create a repository in GitHub without README.md
Note: These instructions works on BASH terminal on Windows & Mac terminals.

Exercise
Create a new repository (it’s a container where all stuff goes) using the + sign as shown below:
image

Provide the necessary details like repository name. Select repository as Public and initialize the READMD. Click ‘Create’.
image

Now, your repository is created, and it looks as:

image

To download the repository, we have option'Download Zip' in 'Code'. Also, there are two options to copy repository locally using ‘SSH’ and ‘HTTPS’
image image

Copy the SSHRepositoryLink on to your clipboard.

Open the command prompt or terminal to use the GitHub commands:

-To change the directory simply use:

cd <name of the directory you want to change to>

-To go to the folder “Downloads” use: cd Downloads

Use the SSH repository link from out GitHub Repository and clone it to your local system as follows:

git clone pastesshrepositorylinkhere

image

Now, the folder is copied to my ‘Downloads’. Just check the ‘Downloads’ have you got the folder demo.

To check my folder, enter the folder using cd command again as: cd demo
Get the list of the files in the folder demo, use: For Windows: dir For Mac: ls

image

To view the content of the file: For Windows: type README.md For Mac: cat README.md

To open a README.md file: For Windows: notepad README.md For Mac: open README.md

To create a new file: For Windows: notepad test.txt For Mac: vi test.txt

Add to the repository: For Windows/Mac: git add test.txt

Check the status of the file using: git status
image

Commit the changes in the repository using: git commit -m “write message here”
image

Push the file to remote repository using: git push
image

Now, this make the changes in my GitHub repository

image

Create a repository now without README.md file
image

Copy the SSHRepositoryLink on to your clipboard as did before

To come out from the demo folder first use cd ..

To make a directory in download folder: mkdir demo1 cd demo1

image

To create a readmd file use echo "# demo1" >> README.md

Initialize the directory git init

Create and add a README.md file. You can use a normal text editor depending on which OS you are using. git add README.md

Check the status of the file git status

Commit the changes git commit -m "first commit"

Add the origin where we have to push the file. This is the SSHRepositoryLink you copied when you created the repository. git remote add origin git@github.com:mskill/demo1.git

Push the file git push -u origin master
image

Now, the README.md file is created in our repository

image

Author(s)
Malika Singla
Other Contributor(s)
Lavanya

Changelog
Date	Version	Changed by	Change Description
2020-08-25	2.0	Lavanya	Migrated Lab to Markdown and added to course repo in GitLab
© IBM Corporation 2020. All rights reserved.
