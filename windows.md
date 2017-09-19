## Windows Setup For Cross-Platform Development

Note: I use Parallels Desktop to use Windows 10 on Mac. Please feel free to use your own virtual machine software.

### Package Management

* [Chocolatey](https://chocolatey.org): "The sane way to manage software on Windows"

### Terminals, shells, and files

#### To install

* [cmder](http://cmder.net/): "a software package created out of pure frustration over the absence of nice console emulators on Windows. It is based on amazing software, and spiced up with the Monokai color scheme and a custom prompt layout, looking sexy from the start."
* [Gow](https://github.com/bmatzelle/gow): "The lightweight alternative to Cygwin"
* [posh-git](https://github.com/dahlbyk/posh-git)

#### powershell profile

run notepad $profile.CurrentUserAllHosts to edit it.
  
    Import-Module posh-git in the file
    New-Alias ll Get-ChildItem

The above will
* import posh-git module
* create an alias of "ll", to do "dir"


### Node

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

```
cinst visualstudiocode
cinst visualstudio2017community
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
