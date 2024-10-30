## Remove previous config:
`
rm -rf ~/.config/nvim
rm -rf ~/.local/share/nvim
`
## Install new config:
`
cd ~/.config/
git clone https://github.com/brianakl/nvim.git
`
### Install packer
`
git clone --depth 1 https://github.com/wbthomason/packer.nvim\
 ~/.local/share/nvim/site/pack/packer/start/packer.nvim
`
then go to lua/brain/packer.lua and remove require('kanagawa'), run :so, quit and reopen nvim, then put kanagawa back

Install fugitive.nvim
`
mkdir -p ~/.vim/pack/tpope/start
cd ~/.vim/pack/tpope/start
git clone https://tpope.io/vim/fugitive.git
vim -u NONE -c "helptags fugitive/doc" -c q
`
 
