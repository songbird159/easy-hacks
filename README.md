# PowerLevel9k to terminal!
### Install ZSH
~~~
sudo dnf install -y zsh
~~~

### Install Oh My ZSH
#### https://github.com/robbyrussell/oh-my-zsh
~~~
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
~~~
### Install PowerLevel9k
#### https://github.com/Powerlevel9k/powerlevel9k/wiki/Install-Instructions#option-2-install-for-oh-my-zsh
~~~
git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k
~~~
#### For root
Does the same then change the default shell by:
~~~
# chsh -s $(which zsh) root
~~~
### Install Hack font
1. Download HACK font from link below
~~~
https://github.com/ryanoasis/nerd-fonts/raw/master/patched-fonts/Hack/Regular/complete/Hack%20Regular%20Nerd%20Font%20Complete.ttf
~~~

2. Install the font
3. Add as default font to your terminal

### Reference
[GNOME 3.28] PowerLevel9k -  The Most Cool Linux Shell EVER!
https://youtu.be/wM1uNqj71Ko

### Colorful less tool

1. Install python3-pygments
~~~
sudo dnf install python-pygments
~~~ 
2. Create file [.lessfilter](https://raw.githubusercontent.com/ehvs/vim_bash_settings/master/.lessfilter) in $HOME dir.
3. In your $HOME/.bashrc add
~~~
export LESS='-R'
export LESSOPEN='|~/.lessfilter %s'
~~~ 
4. Make ~/.lessfilter executable by running
~~~ 
chmod u+x ~/.lessfilter
~~~ 

### Install packages

~~~
sudo dnf install -y bat googler
~~~
