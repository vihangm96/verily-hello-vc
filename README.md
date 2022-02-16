# verily-hello-vc

Hello T9Hacks! Welcome to Verily's Introduction to Version Control talk. Today, we'll be walking you through the basics of how to use Github for Version control.

## Prerequisite: Sign up for a Github account and install Git

Git installation: https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

## Make a repo

If you want to utilize the benefits of version control, you'll need to start by creating a basic organizational unit for the software you want to write: a _repo_.

1. Click on the plus icon in the upper right of any page on GitHub.
2. Click on "New repository".
3. Pick a repository name and add a description.

**NOTE:** Remember to make your repository name short, concise, and descriptive. You'll thank yourself later!

4. Pick a privacy setting (recommended to pick 'Public' for this activity).
5. Initialize the repo.

  - Adding a README provides space for documenting what your code will do.
  - Adding a .gitignore file ensures you don't accidentally commit files you didn't want to.
  - Open source licensing is optional for this activity. We've added a link to the extra credit if you'd like to learn more.

6. Click on "Create repository". You should be taken to the landing page of your repository.

## Clone your repo locally

In this section, we'll show you how to pull this repo down locally so you can write the code in a more convenient environment than the web text editor.

**NOTE:** This section provides instruction on how to clone your repository with SSH. If that isn't working for you, feel free to clone with the HTTPS option instead. (Currently, SSH is considered best practice for security reasons.)

- Click on the "Clone" button in the upper right corner of your newly created repository, then choose the SSH option.
![Screenshot of cloning.](images/EN8ApWcsfWh3MmZ.png)
- Create a key if you don't have one. To do this, start by going into your settings and clicking on "SSH and GPG keys". There should be an option to add a new key, which will take you to this page:
![Screenshot of new SSH key form.](images/6Du2Lgm3QoTLexj.png)
From there, follow these directions to construct an SSH key: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent. After you've generated a key locally, use the Linux `cat` command to output the file to your terminal. Copy the output and paste into the new SSH key box that we saw earlier.
- Follow these directions to test your SSH connection: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/testing-your-ssh-connection
- Finally, you can clone the repo locally! Go back to the main page of this repository and copy the SSH clone link, like this:
![Screenshot of clone URL.](images/A2tYQba5BZw6ZYY.png)
Go back to your command line and type `git clone `, then the link you copied. You should be able to see this repo cloned into your home directory (or anywhere you choose to place it).

## Make a branch

One of the most powerful features that developing code with version control offers is the ability to try experiments on your code and save the results without making potentially disasterous changes to your production code. This ability is enabled via _branching_. In this section, we'll walk through creating a branch for code.

- If you haven't already, change directory into the repository you cloned using the `cd` command on the command line.
- To create a branch, use the command `git branch <your branch name>`. For the purposes of this talk, you'll want to name your branch in the format `<first name>-<last name>-<date of birth>`. You can check it was created by running the `git branch` command without any options and checking that the output contains the name of your branch.
- To move into your code branch, you can use the command `git checkout <your branch name>`.

**TIP:** You can combine the above two commands into one with the syntax `git checkout -b hello-vc-<branch name>`.

## Make a commit and create a pull request

You can save changes to your code by making commits. Let's walk through a typical process of making a change and committing it. (Before you start, make sure you're still in the branch you created above!)

- Start by creating a new file, using `touch hello.py` or a command of your choice.
- Using the command `git status`, you can see the new file you created and a notation of its status. "Untracked" indicates the addition of a new file. If instead you had chosen to change an already existing file (like the README), the file would be listed as "Modified".
- To add all changed files to the list, use the command `git add .` If you only want to add a specific file to the commit, replace the `.` with the file name.
- Next, you'll need to add the commit to your history. You can use the command `git commit -m <something descriptive>` for this.
- Finally, you'll be able to create a pull request for your commit! The command is `git push origin <your branch name>`. You'll see a link in the terminal to create a pull request on Github. Follow the link and fill out the form.

## Find a friend to approve your pull request!

Here at Verily, we very strongly believe in the concept of _two-party control_. The basic idea behind this is that no one person should be able to make a possibly devastating change to the codebase--instead, all changes must be approved by two parties. Version control enables this by implementing an approval mechanism; we'll walk you through how Github does this.

1. Click on the upper right of your new pull request. You should see an option to request a review on the PR you just created. Turn to the person next to you and ask them for their Github username, then add them as an approver.
2. When you get a pull request to approve, ...

## Merge your PR

(CI/CD)

## Optional: fix a commit that went wrong

So far in this tutorial, we've mostly discussed the happy path: you code something cool, then submit it for review.

## Optional: fix a merge conflict

## Cleanup

To keep your local clone neat and tidy, you'll want to wrap up your development for the day with some cleanup. You can delete your working branch with the option -D (as in, `git branch -D <branch-name>`) and update your local clone using the `git pull` command, which pulls the latest code from the remote repository.

## Extra credit
- How version control works: <>
- Open source licensing link: <>
- SSH crypto link: <>
