## Mac For Development

#### Homebrew
https://brew.sh/

"Homebrew installs the stuff you need that Apple didn’t."

#### iterm2
https://www.iterm2.com/

"a replacement for Terminal and the successor to iTerm. It works on Macs with macOS 10.8 or newer. iTerm2 brings the terminal into the modern age with features you never knew you always wanted."

```
brew cask install iterm2
```

#### Oh My Zsh
https://github.com/robbyrussell/oh-my-zsh

```
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

#### Finder, show / hide hidden files
https://ianlunn.co.uk/articles/quickly-showhide-hidden-files-mac-os-x-mavericks/

It's very handy to have alias to turn on / off shwoing hidden files

```
alias showFiles='defaults write com.apple.finder AppleShowAllFiles YES; killall Finder /System/Library/CoreServices/Finder.app'
alias hideFiles='defaults write com.apple.finder AppleShowAllFiles NO; killall Finder /System/Library/CoreServices/Finder.app'
```

##### aliases
https://www.digitalocean.com/community/tutorials/an-introduction-to-useful-bash-aliases-and-functions

```
alias ll="ls -lhA"
```


#### VS Code

```
brew install openssl
```

#### Node.js
https://yarnpkg.com/en/docs/install
```
brew install yarn
```
