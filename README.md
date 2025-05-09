# Git Project
##To remove branch locally
git branch -d (name of branch) safe delete
git branch -D (name of branch) Force delete


##To remove branch remotely
git push origin --delete branch-name
--------------------------------------------------------------------
Difference between annotated tag and Lightweight tag


1. Annotated Tags
Annotated tags are full Git objects stored in the repository. They are the recommended type for marking official release points.

Characteristics:

Include metadata such as the tagger’s name, email, and date.

Can include a descriptive message.

Can be signed with GPG for verification.

Display full details when using commands like git show. 



2. Lightweight Tags
Lightweight tags are simple references to specific commits. They do not contain any additional metadata and are typically used for local or temporary purposes.

Characteristics:

Do not store any additional metadata.

Cannot include a message.

Cannot be signed.

Simpler and faster to create.

----------------------------------------------------------------------
When to use Rebase
git rebase is a powerful command in Git used to streamline a sequence of commits. 

It is commonly used to maintain a clean, 

linear project history by integrating changes from one branch into another.
----------------------------------------------------------------------
How to list tag

1. List All Tags

git tag  - This will output a simple list of all tags in the repository.

2. List Tags Matching a Pattern

git tag -l "v1.*" -  This filters tags using a pattern. For example, the command above lists all tags that start with v1..

---------------------------------------------------------------------
How to delete tag remotely and locally

1. Delete a Tag Locally

git tag -d tag-name

2. Delete a Tag Remotely

git push origin --delete tag-name

![Git Logo](https://git-scm.com/images/logos/downloads/Git-Logo-2Color.png)
