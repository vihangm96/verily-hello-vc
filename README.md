# verily-hello-vc

Hello T9Hacks! Welcome to Verily's Introduction to Version Control talk. Today, we'll be walking you through the basics of how to use Github for Version control.

## Prerequisite: Sign up for a Github account and install Git

Git installation: https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

## Make a repo

TODO add screenshots

1. Click on the plus icon in the upper right.
2. Click on new repository.
3. Pick a repository name and add a description.

**NOTE:** Remember to make your repository name short, concise, and descriptive. You'll thank yourself later!

4. Pick a privacy setting (recommended to pick 'Public' for this activity).
5. Initialize the repo.

  - Adding a README provides space for documenting what your code will do.
  - Adding a .gitignore file ensures you don't accidentally commit files you didn't want to.
  - Open source licensing is optional for this activity. We've added a link to the extra credit if you'd like to learn more.

6. Click on "Create repository". Your finished product should look like this:

## Clone this repo locally

Using SSH
- Create a key if you don't have one. Screenshots:
  - https://screenshot.googleplex.com/EN8ApWcsfWh3MmZ
  - https://screenshot.googleplex.com/6Du2Lgm3QoTLexj
Directions: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
- Cat key to command line, then copy into box. Screenshot: https://screenshot.googleplex.com/7GnWYuhcAehYV4S
- Test SSH connection: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/testing-your-ssh-connection
- Git clone: `git clone <>`. Screenshot: https://screenshot.googleplex.com/A2tYQba5BZw6ZYY

TODO intermission to discuss how version control works with cd'ing into .git directory.

## Make a branch
- `cd verily-hello-vc`
- `git checkout -b hello-vc` (creates a new branch and changes into it in one go)

## Make a commit
- `touch hello.py`
- add something to the file (hand out slips of paper with different messages)
- `git status`
- `git add .` (or `git add <file>`)
- `git commit -m <something descriptive>`
- `git push origin hello-vc`

Click on link -> pull request with description.

## Resolve a merge conflict

TODO: figure out merge conflict steps.

## Find a friend to approve your pull request!

## Merge your PR

(CI/CD)

## Extra credit
- Create a private repo and add a friend to it.
- Open source licensing link: <>
- SSH crypto link: <>
