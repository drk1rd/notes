# git

## setup
* change name and email: `git config --global user.name "Your Name"`, `git config --global user.email "yourname@example.com"`
* to use with github, run this command to change default repository to main: `git config --global init.defaultBranch main`
* coloured git output: `git config --global color.ui auto`
* setup ssh key: run this command once to check whether you have a key or not; `ls ~/.ssh/id_ed25519.pub`; if not found, use this to create one; `ssh-keygen -t ed25519 -C <youremail>`; link it with github by copying it from `cat ~/.ssh/id_ed25519.pub`

## using
* git clone
* git add
* git commit
* git push
* git commit --allow-empty -m "Empty commit"
