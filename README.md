# Vim start

## 연결해서 쓰기
```bash
ln -snf `pwd`/vimrc ~/.vimrc
```


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

### You-completeme
```bash
sudo apt install build-essential cmake
sudo apt install python-dev python3-dev
sudo apt install clang
sudo apt install vim-youcompleteme
```

### Go bundle


#### Ref
* [https://golangkorea.github.io/post/vim-go/](vim-go를 이용한 go 개발 환경 구축)
* [https://github.com/socialpercon/getting-start-golang/blob/master/docs/vim-go.md](vim-go 환경 만들기)

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
$ curl https://raw.githubusercontent.com/gyuha/vim-start/master/vimrc > ~/.vimrc
```

Run vim

### Windows

	https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim

위 파일을 다운로드 받아서 설치된 vim의 `autoload` 폴더에 카피 한다.

Run vim and type the following command:

```vim
:PlugInstall
```
