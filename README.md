# apps

* brave browser
* 1password
* homebrew
  * nvm or volta
  * zsh
  * zsh-autosuggestions
  * awscli
  * openconnect
  * google-cloud-sdk (cask)
* webstorm
  * appearance: dracula
  * scheme: material palenight
  * font: operator mono, 12pm, 1.4
* iterm2
* sourcetree
* gpg suite
* sketch
* teams
* slack
* better snap tool
* transmit
* transporter
* flycut
* displaylink manager
* vlc
* cleanmymac x
* postman
* discord
* teams
* slack

# Git shortcuts

* Delete all local branches apart from the selected/current branch: `git branch | grep -v "$(git branch --show-current)" | xargs git branch -D`
* Stash unstaged changes
```shell
gitstashcustom() {
  # stashes staged, leaving unstaged
  git stash --staged

  # stashes unstaged & untracked       
  git stash -u

  # pops staged back (but they're now unstaged)                
  git stash pop "stash@{1}"
 
  git add -A
}

alias stash-unstaged="gitstashcustom"
```
