To clone a repository from GitHub
```
git clone repository_url 
```

temporary : - machine learning link(https://github.com/manyasrinivas2021/AI-BASED-FACIAL-EMOTION-DETECTION-USING-DEEP-LEARNING.git)

Why do we need to use GIT?
- To track the code changes
- To save the changes committed
- To update and revoke the data/ codes

To create account with user name, and email to git
```
git config --global user.name "Vishnu_1029"

git config --global user.email "vishnuvardhanreddy1029@gmail.com"
```

To initialize or to start the git
```
git init
```

To check the files contains in the given git repository
```
git status
```

To add the file into the git repository
```
		git add file_name_with_extention   // for single file adding

		git add --all                      // for multiple file adding

```

To acknowledge the git after the changes committed in the document
```
git commit -m "AddCommitFileName"
```
1. **`git commit`**:
    
    - This is where the magic happens. When you’re ready to save your changes (after editing files, fixing bugs, or adding new features), you perform a commit. It’s like taking a snapshot of your code at a specific moment.
    - Think of it as saying, “Hey, Git, remember this state of my project!”
2. **`-m "AddCommitFileName"`**:
    
    - The `-m` flag stands for “message.” It’s your chance to leave a little love note to your future self (and your collaborators).
    - The text within the double quotes (`"AddCommitFileName"`) is your commit message. It should be concise but informative.
    - In this case, `"AddCommitFileName"` suggests that you’re adding a file (or multiple files) to your project. Maybe you’ve created a new script, added documentation, or included a fancy cat meme. Whatever it is, this message should capture the essence of your change.

To make the changes committed in the files add to the GitHub repository which you have created from the locally stored at git.
To do this in prior you need to create a repository.
Even make sure that you use the above commit command.
```
git remote add origin LinkOfTheParticularRepository

git push origin master
```

# Configuration
- Set user name: git config : git config - -global user. name "Your Name".
- Set email: git config --global user. email "youremaiiöexampte.com".
- Check settings: git config  - -list
- Set default editor: git config - -global core. editor name.
- Set merge tool: git config --global merge.tool vimdiff.
- Set diff tool: git config --global diff.tool meld.
# Repository Setup
- Create new repository: git init
- Clone a repository: git clone  repository url.
- Add remote repository: git remote add "name" "repo - url".
- List remote repositories: git remote -v

# Basic Workflow
- Check status: git status
- Add changes to staging area: git add "file".
- Commit changes: git commit -m "Commit message"
- Push changes: git push Pull changes: git pull.
- Fetch changes: git fetch


## at an initial stage
```
git init
git add .
git commit -m "kjllkndkfja"
git remote add origin "link"
git push 
```
							or
```

git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/vishnu-vardanreddy/namespace.git
git push -u origin main
```
# after the changes
```
git add .
git commit -m "second commit"
git push
```
							or
To do the same thing in VScode
- Once after the changes commited in the vscode you need to save the file.
- As soon as u save it, it shows the M symbol.
- Go to the branch git icon there at the bottom and give a commite message.
- click on the Tick symbol and click yes on the dialouge box.
- click on 3 dot and select the push to option
- it opens the command pallet there paste the github repo link
- When the successfull of commite mesg comes it means everything is done.

