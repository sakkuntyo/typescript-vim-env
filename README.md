# typescript-vim-env

1. このリポジトリの .vimrc を ~/ に入れる
2. vim-plug を入れる

https://github.com/junegunn/vim-plug

- windows
```powershell
iwr -useb https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim |`
    ni $HOME/vimfiles/autoload/plug.vim -Force
```

- linux
```bash
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```

3. vim 開いて :PlugInstall

4. vim 開いて :CocInstall coc-json coc-tsserver

5. この時点でtsファイルの補完等できるはずだが、微妙か、違いがないなら vim バージョン古すぎるので update
