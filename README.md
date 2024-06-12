# ubuntu setup notes
i want to automate stuff, sync stuff, for my linux setup


## git 

ssh keys
- (`sudo apt install git`)
- `ssh-keygen -t ed25519 -C "EMAIL"`
- `cat ~/.ssh/id_ed25519.pub`
- `git config --global user.email "EMAIL"`


## brave
```
sudo apt install curl
sudo curl -fsSLo /usr/share/keyrings/brave-browser-archive-keyring.gpg https://brave-browser-apt-release.s3.brave.com/brave-browser-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/brave-browser-archive-keyring.gpg] https://brave-browser-apt-release.s3.brave.com/ stable main"|sudo tee /etc/apt/sources.list.d/brave-browser-release.list
sudo apt update
sudo apt install brave-browser
```


## obsidian

- https://obsidian.md/download
- `sudo snap install obsidian --classic`
- https://github.com/Britnell/obsidian-synced-vault


## vscode
- https://code.visualstudio.com/docs/setup/linux
- `sudo snap install --classic code`


## node
https://nodejs.org/en/download/package-manager

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
nvm install 20
node -v 
npm -v 
```


# tar

create
`tar -cvf archive.tar directory/`

extract 
`tar -xvf archive.tar`


