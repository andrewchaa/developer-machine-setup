## Mac and Windows Setup For Cross-Platform Development

Note: I use Parallels Desktop to use Windows 10 on Mac. Please feel free to use your own virtual machine software.

### Package Management

* [Homebrew](https://brew.sh/): "Homebrew installs the stuff you need that Apple didn’t."
* [Chocolatey](https://chocolatey.org): "The sane way to manage software on Windows"

### Terminals, shells, and files

* [iterm2](https://www.iterm2.com/): "a replacement for Terminal and the successor to iTerm. It works on Macs with macOS 10.8 or newer. iTerm2 brings the terminal into the modern age with features you never knew you always wanted."
* [cmder](http://cmder.net/): "a software package created out of pure frustration over the absence of nice console emulators on Windows. It is based on amazing software, and spiced up with the Monokai color scheme and a custom prompt layout, looking sexy from the start."
* [Gow](https://github.com/bmatzelle/gow): "The lightweight alternative to Cygwin"

#### Finder 
From https://ianlunn.co.uk/articles/quickly-showhide-hidden-files-mac-os-x-mavericks/

It's very handy to have alias to turn on / off shwoing hidden files

```
alias showFiles='defaults write com.apple.finder AppleShowAllFiles YES; killall Finder /System/Library/CoreServices/Finder.app'
alias hideFiles='defaults write com.apple.finder AppleShowAllFiles NO; killall Finder /System/Library/CoreServices/Finder.app'
```

### Node

on windows
```
cinst nodejs.install

npm install -g npm-windows-upgrade
npm-windows-upgrade
```

### Version Control

on windows
```
cinst git.install
cinst poshgit

# Restart PowerShell / CMDer before moving on - or run
$env:Path = [System.Environment]::GetEnvironmentVariable("Path","Machine") + ";" + [System.Environment]::GetEnvironmentVariable("Path","User")

cinst Git-Credential-Manager-for-Windows
cinst github
```

### Editors: VS Code

on windows
```
cinst visualstudiocode
cinst visualstudio2017community
```

on mac
```
brew install openssl
```

### Ruby
Even if you don't care about Ruby at all, bear in mind that it's preinstalled on OS X (and easy to install on Unix), so many dev tools might be trying to leverage it. For example, GitHub pages are compiled using Jekyll - if you want to get in on that, install Ruby.

```
cinst ruby
cinst ruby.devkit
```

#### Azure Cli
Super duper useful if you're working with Azure at all.
```
npm install -g azure-cli
```

#### AWS Cli
Super duper useful if you're working with Amazon Web Services at all.
```
cinst awscli
cinst awstools.powershell
```

### Basic Tools
You'll recognize many of these names. Nothing here is crazy unique, it's just stuff you probably want installed to have a well-running machine.

```
cinst vlc
cinst GoogleChrome
cinst 7zip.install
cinst sysinternals
cinst DotNet3.5
```

If you're not running Windows 10, also install:

```
cinst DotNet4.0 -- not needed on windows 8
cinst DotNet4.5 -- not needed on windows 10
cinst PowerShell -- not needed on windows 10
```
