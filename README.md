# vimrc

## Install
`git clone --recursive git@github.com:soruly/vimrc.git`
`cd vimrc`
`./link.sh`

## Add new pathogen plugins
`git submodule add https://github.com/tpope/vim-fugitive.git .vim/bundle/vim-fugitive`

## Initial Project From Scratch
```
sudo dnf install git -y
mkdir -p ~/.vim/autoload ~/.vim/bundle
curl -LSso ~/.vim/autoload/pathogen.vim https://tpo.pe/pathogen.vim
git clone https://github.com/vim-airline/vim-airline ~/.vim/bundle/vim-airline
git clone https://github.com/tpope/vim-fugitive.git ~/.vim/bundle/vim-fugitive
git clone https://github.com/vim-airline/vim-airline-themes ~/.vim/bundle/vim-airline-themes
git clone https://github.com/scrooloose/nerdtree.git ~/.vim/bundle/nerdtree
git clone https://github.com/pangloss/vim-javascript.git ~/.vim/bundle/vim-javascript
git clone --depth=1 https://github.com/vim-syntastic/syntastic.git ~/.vim/bundle/syntastic
touch ~/.vim/.editorconfig
vim -u NONE \
-c "helptags ~/.vim/bundle/vim-airline/doc" \
-c "helptags ~/.vim/bundle/vim-fugitive/doc" \
-c "helptags ~/.vim/bundle/vim-airline-themes/doc" \
-c "helptags ~/.vim/bundle/nerdtree/doc" \
-c "q"
```
