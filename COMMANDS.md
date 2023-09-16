# Commands for Bash

### Connect Via [SSH Key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/about-ssh) (LINUX):
- Check if there are keys in your ~/.ssh folder
- To create a fresh ssh key:
  `$ ssh-keygen -t ed25519 -C "your_email@example.com"`
  - If you choose a passphrase, you can use `ssh-agent` to securely save it for multiple uses.
    - `exec ssh-agent bash` to start ssh-agent if its not running. then run `ssh-add`
  - If you want to recreate/add a passphrase, type: `ssh-keygen -p -f ~/.ssh/id_ed25519`
- Copy your id_ed25519.pub file to your clipboard
- Go into github (or any server) settings and add your ssh public key there.
