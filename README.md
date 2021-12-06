# git-commit-vim
A vim/neovim shell script and keymap for linux that allows for automatic git commiting and pushing to an external repository (that has already been initialized).
The shell script detects the current git repository as well as the current branch, and pushes to the 'origin' external repository branch of the same name.

## Dependencies:
- git.
- vim/neovim.

## Installation (vim):
- Add the git.sh script to ' ~/. ' (This can be customized by changing the calling path in the keymap).
- Add the vim keymap from keymap.vim to your .vimrc.
- Initialize the external repo for your git repository.

## Installation (nvim):
- Add the git.sh script to ' ~/.config/nvim/. ' (This can be customized by changing the calling path in the keymap).
- Add the neovim keymap from keymap.vim to init.vim.
- Initialize the external repo for your git repository.

## Instructions:
Use \<leader\>cp with vim/neovim to:
- save current file,
- stage any non-ignored files that have been added to the repository,
- generate a git commit with the current date and time in the message,
- and git push the generated commit to the external git repository.
