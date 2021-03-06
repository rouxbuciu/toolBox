# What dis?

Here you'll find my dotfiles repo, my setup/keybinding preferences, and a fun script for bootstrapping your whole system from fresh. 
All nice and neat.

It's a work in progress, however, and is likely to change frequently.

**Important:** if for some reason you see fit to try some of these things out, please fork the repo and remove things you don't want or need before using them. Don’t blindly use my settings unless you know what a thing does - a lot of this stuff is idiosyncratic to my workflow. Don't blame me if something goes wrong, or behaves how you don't like it. You have been warned.

# Installation

### First things first
- Take a moment and appreciate what an unadulterated, fresh mac looks like. Yeah, it's pretty neat. Let's get to the nitty-gritty.
- Sign in to Apple accounts; set System Preferences.
- Download and install the important stuff:
    - [iTerm 2](https://www.iterm2.com/downloads.html) - set up hotkey shortcut Cmd-Ctrl-T
    - [Karabiner](https://pqrs.org/osx/karabiner/)
- Download apps you want from App Store
    - Xcode
      - Once installed, open to install tools!
    - 1Password (also get safari/crome extension)

### Next, let's setup the terminal becasue this setup breaks automation:
- ZSH
    - Verify that zsh is installed: `zsh --version` (expected result is `zsh 5.4.2`
  or more recent)
    - Additionally, make sure it's the default shell: `echo $SHELL` with expected
  result as `/usr/bin/zsh` or similar
    - If this doesn't work, [install ZSH](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH)
- [Oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh)
    - Run `sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
  in the home directory.
    - Restart iTerm

### Let's get phys... no. Let's get automated!
- In iTerm, in the home directory, copy and paste the following:
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/electricRGB/.dotfiles/master/setup.sh)"`
- Once finished running, quit terminal and reboot computer for a good time!
- Don't forget to run `p10k configure` to configure your prompt.

### XVim - why settle for less!?
- Because of the certificate, these steps should be done manually.
- Rename standard xcode to Xcode-Distribution (if you need a distribution Xcode)
- Download another version of Xcode [from Apple](https://developer.apple.com/download/more/)
- Sign your own [code signing certificate](https://github.com/XVimProject/XVim2/blob/master/SIGNING_Xcode.md)
- Install [XVim2](https://github.com/XVimProject/XVim2)

### Spacemacs
- Spacemacs install instructions if things didn't go right otherwise: https://github.com/syl20bnr/spacemacs (Install dev branch (if stable))

### Almost done!
- Run `brew doctor` to see any issues and fix them as needed
- Xcode themes from [here](https://github.com/hdoria/xcode-themes) and [here](http://www.codethemes.net/themes/popular/all) should go in `~/Library/Developer/Xcode/UserData/FontAndColorThemes/` (FontAndColorThemes may not exist.)
- [iTerm2 Themes](https://github.com/mbadolato/iTerm2-Color-Schemes)
- One last restart!

## Other Software
This is a list of the software I usually add afterwards that's not sourced from the App Store. It's here so I can just click to go there making my life easier. In no particular order

### Games
- [8BitDo Ultimate Software](https://support.8bitdo.com/ultimate-software.html)
- [Tetr.io](https://tetr.io/about/desktop/)

### Communication
- [Discord](https://discord.com/new/download)
- [Skype](https://www.skype.com/en/get-skype/)

### Development
- [Arduino](https://www.arduino.cc/en/Main/Software)
- [Dash](https://kapeli.com/dash)
- [GitKraken](https://www.gitkraken.com/)

### Entertainment
- [Spotify](https://www.spotify.com/ca-en/download/mac/)

### Browsers
- [Firefox](https://www.mozilla.org/en-CA/firefox/new/)

### Music
- [Band-in-a-Box](https://www.pgmusic.com/)

### Streaming
- [OBS](https://obsproject.com/download)
- [Slobs](https://streamlabs.com/)

### Utilities
- [Amphetamine](https://apps.apple.com/us/app/amphetamine/id937984704?mt=12)
- [AppCleaner](https://freemacsoft.net/appcleaner/)
- [LoopBack](https://rogueamoeba.com/loopback/)


# Why a dotfiles repo?

Inspired by various members of Github, the dotfile repo is a great way to keep all your preferences the same across all dev environments! Tasty!

Furthermore.... it helps get a system going faster from fresh install to ready for development.

# Why share?
Sharing is caring. We learn from each other 🌷

# License

The contents of this repo are licensed under the [MIT license](https://opensource.org/licenses/MIT).

# Contributing

If you have any ideas or suggestions, feel free to open up an issue or shoot through a pull request! Thanks!

Feel free to fork whenever you want!
