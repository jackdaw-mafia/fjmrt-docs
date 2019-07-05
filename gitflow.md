# Github workflow for our project

## Setup

### One person

Make a new repo on Github with (group-project-name). Then make a new dev branch (can easily be done on github). Add protection rules for master and dev. Require one pull review before merger. Dismiss stale requests. Include all members as admins.

### Everyone

```
git clone <remote-url>
```

In terminal,

```
cd <group-project-name>
```

Now in repo and on master branch.

```
git branch -a
```

shows all branches, remote and local.
Do not work on master branch.

```
git checkout dev
```

to change to dev branch.

### Individual

Pull the most recent version of dev to your local computer.

```
git pull
```

(this is the same as git fetch then git merge)
Make your own feature branch.

```
git checkout -b <your-feature-name>
```

### Do your work.

```
git add <files>
```

or

```

git add .

```

to add all.

```

git commit -m “message”

```

Save remotely to your branch using

```

git push

```

or

```

git push origin <your-feature-name>

```

This should not need a review. It also makes your work available to other team members if they are on your feature branch.
Repeat from **Do Your Work** until your feature is complete (same as we are used to with individual work).

### Send changes to github

When complete and ready to merge with dev, it needs one review.
In github, create new pull request (this is a pull from your computer into github’s remote dev branch).
Wait for review.
Reviewer can then delete the branch from github (follow prompt).
In your own local terminal, also delete the branch.

```

git checkout dev

```

```

git branch -d <your-feature-name>

```

because it is the same as dev for your feature, but you need to make a new branch to then get the most up to date version of the whole dev branch.
Now you are on dev branch. Repeat from **Individual**.

### Notes

git pull can lead to conflicts if two people are changing the same file at the same time.

```

git log —help

```

shows how to find your repo history.

git push from your terminal is the same as git pull from github (I think!)
