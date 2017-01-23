# A lightweight customized vim configuration

This is my customized vim configuration.  

It contains some useful plugins, like NERDTree, and some handy settings, like automatically setting a tab to four spaces.

<h1>Dependencies</h1>

The following packages must be installed first:

<ul>
  <li>vim-plug -- Installation instructions here: https://github.com/junegunn/vim-plug
  <li>For YouCompleteMe you will need cmake, clang, and libclang-3.8:
  <ul>
    <li>sudo apt-get install cmake</li>
    <li>sudo apt-get install clang</li>
    <li>sudo apt-get install libclang-dev</li>
  </ul>
</ul>

<h1>Installation</h1>

Installing this configuration is easy:

<ul>
  <li>Clone this repository and copy the .vimrc file to your home directory.
  <li>Open vim.
  <li>Type ':PlugInstall'
  <li>Navigate to ~/.vim/plugged/YouCompleteMe and run: 
    <ul><li>install.py --clang-completer</li></ul>
</ul>

All done!
