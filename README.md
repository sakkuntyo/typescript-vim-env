# Vim でも TypeScript を描きたい

## した事

1. このリポジトリの .vimrc を ~/ に入れる
2. vim-plug を入れる

https://github.com/junegunn/vim-plug

- windows
```powershell
iwr -useb https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim |`
    ni $HOME/vimfiles/autoload/plug.vim -Force
```

- linux (公式)
```bash
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```

---

- linux dasasaki専用(vim)
```
curl -fLo ~/.vim/autoload/plug.vim --create-dirs https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
apt install software-properties-common -y
apt update
add-apt-repository ppa:jonathonf/vim
apt update
apt install vim
```

3. vim 開いて :PlugInstall

4. vim 開いて :CocInstall coc-json coc-tsserver

5. この時点でtsファイルの補完等できるはずだが、微妙か、違いがないなら vim バージョン古すぎるので update

## 表示例
![image](https://user-images.githubusercontent.com/20591351/232804201-38214092-a89a-4d8a-b8fc-a5ab77ce6c2a.png)
