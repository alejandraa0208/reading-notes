# Version Control with Git and Github Notes

## What is GIT?


- It is a version control system where sharing code and collaboration is the goal.
- Keep all of your projects in one repository

### Snapshots

Every time you save a changed version of your project it is called commit.
HEAD = The label meaning \"you are here"

## What is a Version Control System? 

- A system that is able to track modifications

### Without Version Control 

Look familiar? 

- term_paper.docx
- term_paper.docx
- etc.
Creation of multiple files instead of just tracking changes.

## What is Github? 

- Not git \(version control) and github \(online storage code) way to share code online

## Repositories 

A collection of files/folders that youve told Git to pay attention to 

- Usually, one project = one repository
- Really large projects might have mutliple repositories for different parts of their system \(ie: front end vs back end)
- Repositories can live on Github

### Cloning repositories

The command to create a copy of an existing Git repository is

\$ git clone URL 

THe command to close a repo into a diirectory with another name is

\$ git close URL preferred name

## gitflow:acp = add, commit, push 

## Reflection and Discussion Questions 

1. What is version control?

- A system that is able to track project modifications

2. What is cloning in Git?

- Copying all versions of all files for a project

3. What is the command to track and stage files?

- \$ git add file name 
- \$ git add *

4. What is the command to take a snapshot of your changed files? 

- \$ git commit -a

5. What is the command to send your changed files to Github? 

- \$ git push origin master