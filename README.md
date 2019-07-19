# ethan-vim-config
# install vim 
```bash	
//install vim with source code
git clone https://github.com/vim/vim.git
//enable python support
./configure --prefix=/usr/local/ --with-features=huge --enable-multibyte --enable-pythoninterp=yes --with-python-config-dir=/usr/lib/python2.7/config/ --enable-python3interp=yes --with-python3-config-dir=/usr/lib/python3.4/config
//compile and install
make && sudo make install
```
# install vundle
```bash
mkdir -p .vim/bundle
git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
# apply my vimrc
```bash
// this step generally cost much time  due to the YouCompleteMe is quite large
:PluginInstall
// After downloading all plugins, you need to make sure if the essential tools were installed on your machine. 	
sudo apt-get install -y build-essential
// install YouCompleteMe
./install.py --all
```

