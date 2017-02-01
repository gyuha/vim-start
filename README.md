# Vim start
## Pre-requisites

The distribution is designed to work with Vim >= 7.4.

### Mac OSX

```bash
$ brew install git ctags
```

### Linux

* Ubuntu\Debian

```bash
$ sudo apt-get install git exuberant-ctags ncurses-term curl
```

* Gentoo
```bash
$ sudo emerge --ask dev-util/ctags sys-libs/ncurses dev-vcs/git dev-python/pyflakes net-misc/curl
```

* Arch Linux via *pacman* (recomend used *pacaur*)
```bash
$ sudo pacman -S git-core ctags ncurses curl
```
* Fedora

```bash
$ sudo dnf install ncurses-devel git ctags-etags curl
```

### Python bundle (optionally)

* pyflakes
* jedi
* neovim (neovim only) 

```bash
$ pip install flake8 jedi
$ pip2 install --user --upgrade neovim
$ pip3 install --user --upgrade neovim
```

### Windows

Install Git for Windows.

[https://git-scm.com/download/win](https://git-scm.com/download/win)

Open windows powershell.
```powershell
md ~\vimfiles\autoload
$uri = 'https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
(New-Object Net.WebClient).DownloadFile($uri, $ExecutionContext.SessionState.Path.GetUnresolvedProviderPathFromPSPath("~\vimfiles\autoload\plug.vim"))
```

## Install
### Linux & OSX
```bash
$ curl -fLo https://raw.githubusercontent.com/gyuha/vim-start/master/vimrc ~/.vimrc
```

### Windows
```powershell
cd [vim install path]
$uri = 'https://raw.githubusercontent.com/gyuha/vim-start/master/vimrc'
(New-Object Net.WebClient).DownloadFile($uri, $ExecutionContext.SessionState.Path.GetUnresolvedProviderPathFromPSPath("vimrc"))
```

## Vim run
Run vim and type the following command:
```vim
:PlugInstall
```