# Git Credentials on Linux
```bash
sudo apt-get install libgnome-keyring-dev

sudo make --directory=/usr/share/doc/git/contrib/credential/gnome-keyring

git config --global credential.helper /usr/share/doc/git/contrib/credential/gnome-keyring/git-credential-gnome-keyring
```

# Speed up git
`git config --global core.preloadindex true`
`git config --global core.fscache true`
`git config --global gc.auto 256`

# Download submodules
`git submodule update --init --recursive`

# Update submodules
`git submodule update --remote --merge`