# configs
My Personal Configuration files

## Install Scoop and utilities
`iwr -useb get.scoop.sh | iex`

`scoop install curl sudo jq neovim gcc`

## Install Git for Windows
`winget install -e --id Git.Git`

## Create PowerShell config file
```
mkdir .config/powershell
nvim .\.config\powershell\user_profile.ps1
```
The full config file is shared in the repo.

## Point PowerShell config to custom config file
`nvim $PROFILE.CurrentUserCurrentHost`

`. $env:USERPROFILE\.config\powershell\user_profile.ps1`

## Install modules

### oh-my-posh
`winget install oh-my-posh`
### posh-git
`Install-Module posh-git -Scope CurrentUser -Force`
### Terminal-Icons
`Install-Module -Name Terminal-Icons -Repository PSGallery -Force`
### z
`Install-Module -Name z -Force`
### PSReadLine
`Install-Module -Name PSReadLine -AllowPrerelease -Scope CurrentUser -Force -SkipPublisherCheck`
### fzf
`scoop install fzf`
### PSFzf
`Install-Module -Name PSFzf -Scope CurrentUser -Force`
