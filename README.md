# verily-hello-vc

Hello T9Hacks! Welcome to Verily's Introduction to Version Control talk. Today, we'll be walking you through the basics of how to use Github for Version control.

## Prerequisite: Sign up for a Github account and install Git

Git installation: https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

We also need to add you as a collaborator to the Github project.

## A. Setup SSH and Fork Repo 

In this section, we'll show you how to pull this repo down locally so you can write the code in a more convenient environment than the web text editor.

> **NOTE:** 
> * This section provides instruction on how to clone your repository with SSH.
>   * If that isn't working for you, feel free to clone with the HTTPS option instead.
>   * SSH is considered best practice for security reasons, and once configured it is very convenient in practice too!
> * If you already have an ssh key configured with your GitHub account, skip ahead to step 10 below.

1. [Create your ssh key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent), e.g. open a command line (with terminal on Linux and MacOS or Git Bash on Windows) and run `ssh-keygen -t ed25519` while accepting all the defaults by hitting the enter key at each prompt as shown below:

```
$ ssh-keygen -t ed25519
Generating public/private ed25519 key pair.
Enter file in which to save the key (/home/jdimatteo/.ssh/id_ed25519): 
Enter passphrase (empty for no passphrase): 
Enter same passphrase again: 
Your identification has been saved in /home/jdimatteo/.ssh/id_ed25519
Your public key has been saved in /home/jdimatteo/.ssh/id_ed25519.pub
```

2. Copy your **public** key to the clipboard, e.g. back on the command line run `cat ~/.ssh/id_ed25519.pub` then select the printed line and copy it to your clipboard (CTRL-SHIFT-C on Linux and Windows or CMD-C on MacOS). The text should be a long line starting with `ssh-ed25519`. Paste this text to  After you've generated a key locally, use the Linux `cat` command to output the file to your terminal.

3. Open your [GitHub user settings](https://github.com/settings/profile)

![image](https://user-images.githubusercontent.com/3752732/154405056-d9683886-7f9b-49fd-bd6f-983eaf75f498.png)

4. Drill down to [SSH and GPG keys](https://github.com/settings/keys)

![image](https://user-images.githubusercontent.com/3752732/154405195-5e092bd7-3511-487b-99c6-2d2ce1817b1f.png)

5. Click [New SSH key](https://github.com/settings/ssh/new)

![image](https://user-images.githubusercontent.com/3752732/154405268-3a8ba4fa-4bd2-4708-82ab-4535a52bdc06.png)

6. Paste your public key (copied to the clipboard in step #2) to the "Key" text box:

![image](https://user-images.githubusercontent.com/3752732/154407383-de2ff24f-6ea8-48ad-8e7e-4f477f53bcbd.png)

7. Click "Add SSH Key"

![image](https://user-images.githubusercontent.com/3752732/154407488-32385a1d-6d29-4d43-bf21-e43586a1c100.png)

8. Follow these directions to test your SSH connection: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/testing-your-ssh-connection

9. Finally, you can clone the repo locally with ssh! Go back to the main page of this repository (if you are having trouble finding it, click [Your repositories](https://user-images.githubusercontent.com/3752732/154408379-c6d2c9c5-9b9e-4140-83e5-f3958f4b57c1.png)) and click on the Fork button. This creates a new repo that you own.

10. Click on the "Clone" button in the upper right corner of your newly created repository, then choose the SSH option, then click the copy to clipboard button, like this:

![image](https://user-images.githubusercontent.com/3752732/154408715-d6b88db5-e738-4e73-8768-eabab5bccee6.png)

10. Go back to your command line and type `git clone ` followed by pasting your clipboard (CTRL-SHIFT-V on Linux and Windows or CMD-V on MacOS).

11. You should now be able to see this repo cloned into your home directory (or anywhere you choose to place it).

## B. Fork the Repo and Create a Pull Request

1. Go to https://github.com/KilimAnnejaro/verily-hello-vc ([t.ly/ZqjP](https://t.ly/ZqjP)).

2. Click the fork button in the top right

![image](https://user-images.githubusercontent.com/3752732/154769938-56171260-59c6-45ec-a1bd-a5ff1caebfce.png)

3. Wait until fork completes

![image](https://user-images.githubusercontent.com/3752732/154769926-ede99504-1401-4735-8618-0dc5dee39a9b.png)

4. Click `favorite_built_in_modules.py`

![image](https://user-images.githubusercontent.com/3752732/154770639-cf908545-27fd-47fc-b5b0-cb66f1e9c78e.png)

5. Click the edit button

![image](https://user-images.githubusercontent.com/3752732/154770729-2a52ad14-eee5-40af-bfc3-9f6c96add60e.png)

6. Make your changes

Just for an example, lets pretend we wanted to share our favorite python built in modules with a program like this.

All of us will add to this file, what our favorite module is, e.g.

![image](https://user-images.githubusercontent.com/3752732/154771299-e7f0cddb-b715-4308-9794-22b3153f93b0.png)

7. Add a commit message

![image](https://user-images.githubusercontent.com/3752732/154771346-87fe1ad2-2287-4181-a672-14bc18de60ca.png)

8. Commit directly to your fork's main branch

![image](https://user-images.githubusercontent.com/3752732/154771652-8a9cdb0d-5f8c-4043-bb4c-c0e9d3b850bc.png)

9. Click "Commit changes"

![image](https://user-images.githubusercontent.com/3752732/154771665-119b9b65-6e34-413d-ac6d-5de3dd3b028d.png)

10. Go back to the original repository

![image](https://user-images.githubusercontent.com/3752732/154771703-fd6e8243-6256-448f-bc51-39d66ca9eda1.png)

11. Click "Compare & pull request"

 ![image](https://user-images.githubusercontent.com/3752732/154771736-96ce3f1f-d217-4f3b-9132-8f6e587b01d4.png)

12. Click "Create pull request"

![image](https://user-images.githubusercontent.com/3752732/154771790-1c45cb8c-dce9-4c10-80e3-42dddfe43d69.png)

## C. Code Review

1. Find a buddy to review each other's code.

2. Ask your buddy to open the pull request

![image](https://user-images.githubusercontent.com/3752732/154772146-009552f1-32dc-4d71-9c67-6bd625f0ea38.png)

3. Click "Files changed" then "Review changes"

![image](https://user-images.githubusercontent.com/3752732/154772209-1f27f5b7-8ca8-449c-9de7-b79f026c7de9.png)

4. Write a message then click "Submit review"

![image](https://user-images.githubusercontent.com/3752732/154772263-31889fe5-3a34-4242-9455-f4c46f610c44.png)

5. Once reviewed, ask Annie or John to merge the PR

## D. Conflicts

Some of you will encounter conflicts:

1. Conflicts look like this:

![image](https://user-images.githubusercontent.com/3752732/154773203-625f67f2-d108-4c47-b94b-06d411d1b9d8.png)

2. Resolve your conflicts inline:

![image](https://user-images.githubusercontent.com/3752732/154773247-69256fb2-87a4-4e5d-b8f4-4e5ba393c209.png)

## E. Optional: fix a commit that went wrong

So far in this tutorial, we've mostly discussed the happy path: you code something cool, then submit it for review. But what happens if you submit a commit you don't want? Version control with git offers us a way to fix this issue!

Prerequisite: creating a commit that you don't like.

1. Run the command `git log` to print a list of all commits, then copy to clipboard the hash of the commit preceding the one you want to remove. Type `q` at the command prompt to return to your command line interface.
2. There are a lot of ways to roll back commits you don't want; some of them are detailed at <https://stackoverflow.com/questions/4114095/how-do-i-revert-a-git-repository-to-a-previous-commit>. In this lesson, we're going to assume that you don't want your bad commit at all and that you never want to see it again.
3. The command for completely wiping out your bad commit is `git reset --hard <hash-1>` where `<hash-1>` is the hash of the commit preceding the one you want to remove.
4. If you've already pushed bad code to a pull request, you can use the force push option to push the branch with the bad commit removed to origin. The command is `git push -f origin <branch-name>`.

## F. Cleanup

To keep your local clone neat and tidy, you'll want to wrap up your development for the day with some cleanup. You can delete your working branch with the option -D (as in, `git branch -D <branch-name>`) and update your local clone using the `git pull` command, which pulls the latest code from the remote repository.

## J. Extra credit
- How version control works: <https://git-scm.com/book/en/v2/Git-Internals-Plumbing-and-Porcelain>
- Open source licensing link: <https://opensource.org/faq>
