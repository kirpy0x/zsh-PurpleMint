A Purple & Teal ZSH theme
======

![alt tag](https://raw.githubusercontent.com/kirpy0x/zsh-PurpleTeal/master/demo.png)


Powerline looking zsh theme with rvm prompt, git status and branch, current time, user, hostname, pwd, exit status, root and background job status.

Influenced heavily by [agnoster's theme](https://gist.github.com/3712874) and [jeremyFreeAgent's theme](https://github.com/jeremyFreeAgent/oh-my-zsh-powerline-theme)

Forked from [consolemaverick](https://github.com/consolemaverick/zsh2000)

### Prerequisites

My Terminal: Kitty

My Font: ComicMono

### Installation

Past this into your `.zshrc`.
```sh
# Install if not already installed
if [ -f ~/.oh-my-zsh/custom/themes/PurpleTeal.zsh-theme ]; then
else
  git clone https://github.com/kirpy0x/zsh-PurpleTeal.git ~/.oh-my-zsh/custom/themes/PurpleTeal
  mv ~/.oh-my-zsh/custom/themes/PurpleTeal/PurpleTeal.zsh-theme ~/.oh-my-zsh/custom/themes/PurpleTeal.zsh-theme
  rm -rf ~/.oh-my-zsh/custom/themes/PurpleTeal
fi
# Enable
ZSH_THEME="PurpleTeal"
```

### Configuration

Disable the right hand side prompt entirely

    export ZSH_2000_DISABLE_RIGHT_PROMPT='true'

Disable user@hostname

    export ZSH_2000_DEFAULT_USER='YOUR_USER_NAME'

Disable display of

1. exit status of your last command
2. whether or not you are root
3. whether or not there are background jobs running

by adding

    export ZSH_2000_DISABLE_STATUS='true'

Disable git status on top of plain git clean/dirty

    export ZSH_2000_DISABLE_GIT_STATUS='true'

Disable RVM prompt

    export ZSH_2000_DISABLE_RVM='true'
