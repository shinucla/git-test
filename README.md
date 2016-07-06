# git-test

// working with SSH

1) Generating an SSH key
   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

   # should you use github login email? maybe

   # enter where to save? /Users/you/.ssh/github_id_rsa

   # enter passcode or not? maybe not

2) Adding your SSH key to the ssh-agent
   # start the ssh-agen in the background
   $ eval $(ssh-agent)
   Agent pid 3433

   $ ssh-add ~/.ssh/github_id_rsa

3) Adding a new SSH key to your GitHub account

   In the top right corner of any page, click your profile photo, then click Settings.

   In the user settings sidebar, click SSH and GPG keys.

   Click New SSH key.

   In the "Title" field, add a descriptive label for the new key. 

   Paste the content of github_id_rsa.pub into the "Key" field.

   Click Add SSH key.

4) Testing your SSH connection
   $ ssh -T git@github.com
   # Attempts to ssh to GitHub
 


// using git

1) install: sudo apt-get install git

2) clone:
   $ git clone your-git-project-ssh-path
   # this will create a folder with your project name at current directory




