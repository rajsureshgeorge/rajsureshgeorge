
# Table of Contents

1.  [Git Adding Commands](#orgfcbba77)
    1.  [Adding a file](#org3123b00)
    2.  [Adding Every file](#org5e6d2fb)
    3.  [Updating Already Staged files](#org6543bfb)
    4.  [Save Change in the entire working directory](#org8a6f581)
2.  [Git Branch Commandg](#org10bf295)
    1.  [List Branches](#orgdf4141f)
    2.  [Create a New Branch](#org5887cfd)
    3.  [Switch to a Branch](#org636bafb)
    4.  [Create and Switch to a new branch](#org8da2f1d)
    5.  [Delete a Branch](#orgccc1195)
    6.  [Force Delete a Branch](#orga2b6b76)
    7.  [Rename a Branch](#org8284ea4)
    8.  [Renaming Current Branch name](#org9bce3a7)
    9.  [Track Remote Branch](#org6763e0a)
    10. [List All Branches (Local and Remote)](#orgb7e40ac)
    11. [List Remote Branches](#orga21e104)
3.  [Git Commit Commands](#org463f58f)
    1.  [Commit with a Message](#orgd9b3b26)
    2.  [Commit All Changes](#orga1538ce)
    3.  [Amend Last Commit](#org8532588)
    4.  [Interactive Commit](#orga4f358f)
    5.  [Detailed Commit Message](#org10bb255)
    6.  [Sign-Off a Commit](#orgd86ed7b)
    7.  [Specify Author](#org7243a99)
    8.  [Include Untracked Files](#orgd2926a4)
    9.  [Allow Empty Commit](#orgd5dcc41)
    10. [Commit with GPG Signature](#org509ccd5)
    11. [Commit Using a Template](#org7d823eb)
    12. [Commit with Verbose Output](#org98397ee)
4.  [Git Log Commands](#org4c4376f)
    1.  [Git Log with decoration](#org08505bf)
    2.  [Git log with formatting](#org9cd5a9f)
    3.  [Git log find by commit message](#orga40ef72)
5.  [Git Tag Commands](#org276e234)
    1.  [Normal Git Tagging](#orga08d630)
    2.  [Pushing Git tags](#org4b50ce2)
    3.  [Delete Git Tag](#org05a025d)
    4.  [Tagging with new tag name](#org11b91b1)
    5.  [Pushing the Old Delete tag Update to Origin (local git / gitlab / github](#org963ee75)


<a id="orgfcbba77"></a>

# Git Adding Commands


<a id="org3123b00"></a>

## Adding a file

git add file


<a id="org5e6d2fb"></a>

## Adding Every file

git add .


<a id="org6543bfb"></a>

## Updating Already Staged files

git add -u (or) git add &#x2013;update


<a id="org8a6f581"></a>

## Save Change in the entire working directory

git add -a (or) git add &#x2013;all


<a id="org10bf295"></a>

# Git Branch Commandg


<a id="orgdf4141f"></a>

## List Branches

git branch


<a id="org5887cfd"></a>

## Create a New Branch

git branch <branch-name>


<a id="org636bafb"></a>

## Switch to a Branch

git checkout <branch-name>


<a id="org8da2f1d"></a>

## Create and Switch to a new branch

git checkout -b <branch-name>


<a id="orgccc1195"></a>

## Delete a Branch

git branch -d <branch-name>


<a id="orga2b6b76"></a>

## Force Delete a Branch

git branch -D <branch-name>


<a id="org8284ea4"></a>

## Rename a Branch

git branch -m <new-branch-name>


<a id="org9bce3a7"></a>

## Renaming Current Branch name

git branch -m <old-branch-name> <new-branch-name>


<a id="org6763e0a"></a>

## Track Remote Branch

git branch &#x2013;track <new-branch> <remote-branch>


<a id="orgb7e40ac"></a>

## List All Branches (Local and Remote)

git branch -a


<a id="orga21e104"></a>

## List Remote Branches

git branch -r


<a id="org463f58f"></a>

# Git Commit Commands


<a id="orgd9b3b26"></a>

## Commit with a Message

git commit -m "Your commit message"


<a id="orga1538ce"></a>

## Commit All Changes

git commit -a -m "Your commit message"
      The -a option stages all modified and deleted files before committing, but it does not stage new untracked files.


<a id="org8532588"></a>

## Amend Last Commit

git commit &#x2013;amend -m "Updated commit message"
      The -a option stages all modified and deleted files before committing, but it does not stage new untracked files.


<a id="orga4f358f"></a>

## Interactive Commit

git commit -p
      The -p (or &#x2013;patch) option allows you to interactively select parts of files to commit. This is useful for breaking a large change into smaller, more meaningful commits.  


<a id="org10bb255"></a>

## Detailed Commit Message

git commit
      This command opens the default text editor, allowing you to write a detailed, multi-line commit message.


<a id="orgd86ed7b"></a>

## Sign-Off a Commit

git commit -s -m "Your commit message"
      The -s (or &#x2013;signoff) option adds a Signed-off-by line at the end of the commit message. This is often used in projects that require a Developer Certificate of Origin (DCO).


<a id="org7243a99"></a>

## Specify Author

git commit &#x2013;author="Author Name <email@example.com>" -m "Your commit Message"


<a id="orgd2926a4"></a>

## Include Untracked Files

git commit -a -m "Your cAllow Empty Commituommit message" -o


<a id="orgd5dcc41"></a>

## Allow Empty Commit

git commit &#x2013;allow-empty -m "Empty commit message"


<a id="org509ccd5"></a>

## Commit with GPG Signature

git commit -S -m "Your commit message"
      The -S (or &#x2013;gpg-sign) option signs the commit with your GPG key, providing cryptographic proof that the commit was made by you.


<a id="org7d823eb"></a>

## Commit Using a Template

git commit &#x2013;template=<file>


<a id="org98397ee"></a>

## Commit with Verbose Output

git commit &#x2013;verbose


<a id="org4c4376f"></a>

# Git Log Commands


<a id="org08505bf"></a>

## Git Log with decoration

git log &#x2013;graph &#x2013;oneline &#x2013;decorate &#x2013;all


<a id="org9cd5a9f"></a>

## Git log with formatting

git log &#x2013;graph &#x2013;oneline &#x2013;decorate &#x2013;all


<a id="orga40ef72"></a>

## Git log find by commit message

git log &#x2013;all &#x2013;grep="commit message"


<a id="org276e234"></a>

# Git Tag Commands


<a id="orga08d630"></a>

## Normal Git Tagging

git tag (name)/(version)


<a id="org4b50ce2"></a>

## Pushing Git tags

git push &#x2013;tags


<a id="org05a025d"></a>

## Delete Git Tag

git tag -d (name)/(version)


<a id="org11b91b1"></a>

## Tagging with new tag name

git tag (new<sub>name</sub>) (with<sub>commit</sub><sub>hash</sub>)


<a id="org963ee75"></a>

## Pushing the Old Delete tag Update to Origin (local git / gitlab / github

git push origin :refs/tags/old<sub>tag</sub><sub>name</sub>
