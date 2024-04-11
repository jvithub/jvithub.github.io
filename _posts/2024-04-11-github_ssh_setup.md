# Adding a Local Repository to Github for macOS:

Generating and adding SSH keys only need to be done if it hasn't been done before.

Generate SSH key (if not already done):

    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

Add SSH key to SSH agent:

    eval "$(ssh-agent -s)"

Add SSH private key to the SSH agent:

    ssh-add ~/.ssh/id_rsa
