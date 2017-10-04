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


#### Git

What's a developer without [Git](http://git-scm.com/)? To install, simply run:

    $ brew install git
    
When done, to test that it installed fine you can run:

    $ git --version
    
And `$ which git` should output `/usr/local/bin/git`.

Let's set up some basic configuration. Download the [.gitconfig](https://raw.githubusercontent.com/nicolashery/mac-dev-setup/master/.gitconfig) file to your home directory:

    $ cd ~
    $ curl -O https://raw.githubusercontent.com/nicolashery/mac-dev-setup/master/.gitconfig

It will add some color to the `status`, `branch`, and `diff` Git commands, as well as a couple aliases. Feel free to take a look at the contents of the file, and add to it to your liking.

Next, we'll define your Git user (should be the same name and email you use for [GitHub](https://github.com/) and [Heroku](http://www.heroku.com/)):

    $ git config --global user.name "Your Name Here"
    $ git config --global user.email "your_email@youremail.com"

They will get added to your `.gitconfig` file.

To push code to your GitHub repositories, we're going to use the recommended HTTPS method (versus SSH). So you don't have to type your username and password everytime, let's enable Git password caching as described [here](https://help.github.com/articles/set-up-git):

    $ git config --global credential.helper osxkeychain

#### VS Code

```
brew install openssl
```

#### Node.js
https://yarnpkg.com/en/docs/install
```
brew install yarn
```

### Paralles Desktop

#### Keyboard shotcut

Go to Settings > Shortcuts > Windows 10

* CMD + ->: End, to use Mac shortcut for End on windows. Otherwise, you keep arranging windows
* CMD + <-: Home
