# Adding a Local Repository to Github for macOS:

Generating and adding SSH keys only need to be done if it hasn't been done before.

Generate SSH key (if not already done):

    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

Add SSH key to SSH agent:

    eval "$(ssh-agent -s)"

Add SSH private key to the SSH agent:

    ssh-add ~/.ssh/id_rsa

Copy key to clipboard:

    pbcopy < ~/.ssh/id_rsa.pub

Add the key to 'SSH keys' in settings of Github profile.

Create a new github repository with the name of the local repository.

Initialise the local repository using source tree, or try the command:

    git init .

Add the origin:

    git remote add origin git@github.com:jvithub/ELEC4630_Environment.git

Set the url:

    git remote set-url origin git@github.com:jvithub/ELEC4630_Environment.git

Now we can add, commit and push files.
