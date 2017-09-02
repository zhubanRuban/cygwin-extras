# cygwin-extras
Enhancements for Cygwin-like environments

By default, Cygwin asks for SSH key password on every SSH login
This code will re-use existing SSH agent for every new Cygwin window

Based on http://www.electricmonk.nl/log/2012/04/24/re-use-existing-ssh-agent-cygwin-et-al/
Modified for cygwin-portable-installer from https://github.com/vegardit/cygwin-portable-installer

How to use:
Append to your .bashrc

Configuration:
SSH_AUTH_PATH - a path where SSH agent will store its tmp files, moved to separate folder in $HOME for convenience
                default: ~/.agentssh
SSH_AUTH_KEY  - a path to your SSH key, modify according for this scheme to work
                default: ~/.ssh/id_dsa
