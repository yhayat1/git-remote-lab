# Authenticate to GitHub repo with SSH

1) If not already exists, generate an SSH key using this cmd: ssh-keygen -t ed25519 -C "your_email@example.com"
2) Display the publib SSH key using this cmd: cat ~/.ssh/id_ed25519.pub
3) Copy the public key
4) Navigate to GitHub > Settings > SSH and GPG keys > click on "New SSH key" > Pasth the public key
5) Test the usage of the ssh key by running: ssh -T git@github.com
Expected result:

Hi your-username! You've successfully authenticated...

6) Run git clone with the repo SSH URL and it should be successfully cloned.
