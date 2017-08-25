## Mac and Windows Setup For Cross-Platform Development

Note: I use Parallels Desktop to use Windows 10 on Mac. Please feel free to use your own virtual machine software.

### Package Management

* [Homebrew](https://brew.sh/): "Homebrew installs the stuff you need that Apple didn’t."

### Terminals, shells, and files

* [iterm2](https://www.iterm2.com/): "a replacement for Terminal and the successor to iTerm. It works on Macs with macOS 10.8 or newer. iTerm2 brings the terminal into the modern age with features you never knew you always wanted."
* Finder: https://ianlunn.co.uk/articles/quickly-showhide-hidden-files-mac-os-x-mavericks/

  It's very handy to have alias to turn on / off shwoing hidden files

   ```
   alias showFiles='defaults write com.apple.finder AppleShowAllFiles YES; killall Finder /System/Library/CoreServices/Finder.app'
   alias hideFiles='defaults write com.apple.finder AppleShowAllFiles NO; killall Finder /System/Library/CoreServices/Finder.app'
   ```

 
##### bash aliases




### VS Code

on mac
```
brew install openssl
```

