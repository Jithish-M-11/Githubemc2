# GitHub tutorial vs code:

## IN CMD TO CONFIGURE THE GIT ID:
    git config --global user.name "(GIT username)"
    git config --global user.email "(GIT EMAIL)"

## CLONE:
IN CMD->

    PS C:\Users\jithi\Desktop\youtube git> git clone https://github.com/Jithish-M-11/Githubemc1.git
    Cloning into 'Githubemc1'...
    remote: Enumerating objects: 3, done.
    remote: Counting objects: 100% (3/3), done.
    remote: Total 3 (delta 0), reused 0 (delta  0), pack-reused 0
    Receiving objects: 100% (3/3), done.

## MOVING TO THE NEXT FILE:
CMD->

    PS C:\Users\jithi\Desktop\youtube git> cd
    PS C:\Users\jithi\Desktop\youtube git> cd githubemc1

### CREATE A FILE IN VS CODE(test2.txt) IN CLONED FILE WHERE YOU NEED;

## TO check STATUS: 
    PS C:\Users\jithi\Desktop\youtube git\githubemc1> git status
On branch main
Your branch is up to date with 'origin/main'.
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test2.txt(red).
nothing added to commit but untracked files present (use "git add" to track)

ADDING THE FILE IN LOCAL FOLDER -> git add [file name]:
PS C:\Users\jithi\Desktop\youtube git\githubemc1> git add test2.txt
PS C:\Users\jithi\Desktop\youtube git\githubemc1> git status
On branch main
Your branch is up to date with 'origin/main'.
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   test2.txt(green).


ADDING THE FILE LOCAL FOLDER TO GIT FOLDER-> git commit -m "(COMMENT LINE)":
PS C:\Users\jithi\Desktop\youtube git\githubemc1> git commit -m "Test2.txt file is added"      
[main 8058126] Test2.txt file is added
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test2.txt

## PUSH THE FILE FROM GIT FOLDER TO GIT REPOSITORY:[REPOSITORY BRANCH IS 'main"]
PS C:\Users\jithi\Desktop\youtube git\githubemc1> git push origin main
info: please complete authentication in your browser...
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 288 bytes | 288.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Jithish-M-11/Githubemc1.git
   2e45f0c..8058126  main -> main



## TO REMOVE THE FILE IN GIT REPOSITORY:(USE git rm "filename")

IF you want to remove the file  in git repository and the file system(cloned one).Then,
 USE: 
 	git rm "(FILE NAME)"
	git commit -m "file is removed"
	git push origin (branch name)
If you want to remove the file in git repository and there is no change in file system.Then,
USE:
	git rm --catch (file name)
	git commit -m "(file name")
	git push origin (branch name)


## PULL:
pull is use to if the repo has made any new changes/update in file then using pull we get the changes in file system(windows).then,

USE:

    git pull 


## CREATE a NEW FOLDER in system and try to push in git a new repository:

In path when we try to go back in CMD file path.Then we need to use:

    cd ..

1. INITILIZED EMPTY GIT REPOSITORY
    USE THIS COMMEND:

        git init

2.ADD THE CHANGES CODE:
    i