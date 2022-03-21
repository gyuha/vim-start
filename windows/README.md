# 윈도우용 세팅

`_vimrc` 파일에서 사용 할 경로의 위치를 정해 줍니다.
```
let g:vim_path = $HOME.'\util\vim\vimfiles'
```

위 경로에 아래와 같이 파일을 복사 해 넣어 줍니다.
```
curl -fLo ~/util/vim/vimfiles/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

그리고, vim을 실행 후 아래와 같이 실행을 해 줍니다.
```
:PlugInstall
```







