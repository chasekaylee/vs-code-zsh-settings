# vs-code-zshrc-settings
### will organize later
```
#VS-CODE SETTINGS# 
{
    "editor.matchBrackets": false,
    "sublimeTextKeymap.promptV3Features": true,
    "editor.multiCursorModifier": "ctrlCmd",
    "editor.snippetSuggestions": "top",
    "editor.formatOnPaste": true,
    "workbench.colorTheme": "One Dark Pro Vivid",
    "workbench.fontAliasing": "antialiased",
    "editor.renderWhitespace": "all",
    "editor.renderLineHighlight": "all",
    "editor.tabSize": 2,
    "editor.cursorBlinking": "solid",
    "extensions.ignoreRecommendations": false,
    // Controls the font size in pixels.
    "editor.fontSize": 14,
    // Controls the font family.
    "editor.fontFamily": "Fira Code, Roboto Mono, Menlo, Inconsolata",
    "editor.fontLigatures": true,
    "window.zoomLevel": -1,
    "files.trimTrailingWhitespace": true,
    // The path of the shell that the terminal uses on Linux.
    "terminal.integrated.shell.osx": "/bin/zsh",
    // Controls the font family of the terminal, this defaults to editor.fontFamily's value.
    "terminal.integrated.fontFamily": "Inconsolata for Powerline",
    "workbench.startupEditor": "newUntitledFile",
    "editor.renderIndentGuides": true,
    "window.openFilesInNewWindow": "on",
    "window.openFoldersInNewWindow": "on"
}


#~./zshrc PROFILE#

# If you come from bash you might have to change your $PATH.
# export PATH=$HOME/bin:/usr/local/bin:$PATH

# Path to your oh-my-zsh installation.
export ZSH=/Users/chasekaylee/.oh-my-zsh

# Set name of the theme to load. Optionally, if you set this to "random"
# it'll load a random theme each time that oh-my-zsh is loaded.
# See https://github.com/robbyrussell/oh-my-zsh/wiki/Themes
# POWERLEVEL9K_MODE='nerdfont-complete'
ZSH_THEME="powerlevel9k/powerlevel9k"

# Set list of themes to load
# Setting this variable when ZSH_THEME=random
# cause zsh load theme from this variable instead of
# looking in ~/.oh-my-zsh/themes/
# An empty array have no effect
# ZSH_THEME_RANDOM_CANDIDATES=( "robbyrussell" "agnoster" )

# Uncomment the following line to use case-sensitive completion.
# CASE_SENSITIVE="true"

# Uncomment the following line to use hyphen-insensitive completion. Case
# sensitive completion must be off. _ and - will be interchangeable.
# HYPHEN_INSENSITIVE="true"

# Uncomment the following line to display red dots whilst waiting for completion.
COMPLETION_WAITING_DOTS="true"

export UPDATE_ZSH_DAYS=3

# Uncomment the following line if you want to disable marking untracked files
# under VCS as dirty. This makes repository status check for large repositories
# much, much faster.
# DISABLE_UNTRACKED_FILES_DIRTY="true"

# Uncomment the following line if you want to change the command execution time
# stamp shown in the history command output.
# The optional three formats: "mm/dd/yyyy"|"dd.mm.yyyy"|"yyyy-mm-dd"
# HIST_STAMPS="mm/dd/yyyy"

# Which plugins would you like to load? (plugins can be found in ~/.oh-my-zsh/plugins/*)
# Custom plugins may be added to ~/.oh-my-zsh/custom/plugins/
# Example format: plugins=(rails git textmate ruby lighthouse)
# Add wisely, as too many plugins slow down shell startup.
# if [[ -n $SSH_CONNECTION ]]; then
#   export EDITOR='vim'
# else
#   export EDITOR='mvim'
# fi

# Compilation flags
# export ARCHFLAGS="-arch x86_64"

# ssh
# export SSH_KEY_PATH="~/.ssh/rsa_id"

# Set personal aliases, overriding those provided by oh-my-zsh libs,
# plugins, and themes. Aliases can be placed here, though oh-my-zsh
# users are encouraged to define aliases within the ZSH_CUSTOM folder.
# For a full list of active aliases, run `alias`.

# Example aliases
alias z="vim ~/.zshrc"
alias ohmyzsh="vim ~/.oh-my-zsh"
alias S='source ~/.zshrc'
alias IP='ifconfig -a | grep broadcast'
alias WHO='arp -a'
alias a='pwd'
alias ls='ls -GFh'
alias c='clear'
alias computer='uname -a'
alias brewup='brew update; brew upgrade; brew prune; brew cleanup; brew doctor'
alias gitconfig='nano ~/.gitconfig'
alias sshconfig='nano .ssh/config'
alias dev='cd /Users/chasekaylee/Documents/dev/github/chasekaylee/hackreactor'

## VS CODE ##
code () { VSCODE_CWD="$PWD" open -n -b "com.microsoft.VSCode" --args $* ;}


## POWERLEVEL ##
# Limit to the last two folders
POWERLEVEL9K_SHORTEN_DIR_LENGTH=2

#POWERLEVEL9K_PROMPT_ON_NEWLINE=true
#POWERLEVEL9K_MULTILINE_SECOND_PROMPT_PREFIX="↳ "
#POWERLEVEL9K_DISABLE_RPROMPT=true
# Gets rid of cl@ckl on each command
DEFAULT_USER=`whoami`
```
