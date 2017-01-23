# A lightweight customized vim configuration

This is my customized vim configuration.  

It contains some useful plugins, like NERDTree, and some handy settings, like automatically setting a tab to four spaces.

<h1>Dependencies</h1>

The following packages must be installed first:

<ul>
  <li>vim-plug -- Installation instructions here: https://github.com/junegunn/vim-plug
  <li>For YouCompleteMe and C-family support you will need cmake, clang, and libclang-3.8:
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

<h1>Additional Notes</h1>

In order to use C-family autocompletion with YCM, you will need to define compilation flags for YCM to reference.

Information on how to achieve this can be found here: https://github.com/Valloric/YouCompleteMe/blob/master/README.md#c-family-semantic-completion

To get up and running fast:
<ul>
<li>Create a .ycm_extra_conf.py Python script in your project's root directory.</li>
<li>Add this to it:</li>
<code>def FlagsForFile( filename, **kwargs ):
  return {
    'flags': [ '-x', 'c++', '-Wall', '-Wextra', '-Werror' ],
    }</code>
    <li>Save and close.</li>
    </ul>
