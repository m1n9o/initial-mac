# initial mac

该代码库使用 ansible homebrew 为一个全新的 mac 安装以及配置一个开发常用所需要的软件包和配置。

怎么运行：

```
./run.sh '{you sudo password}'
```

在安装 cask 的时候，有些软件需要 sudo 的密码。

暂时安装了：

cask：

- iterm2
- lastpass
- qqmusic
- visual-studio-code
- zoom
- intellij-idea
- sogouinput
- postman
- ticktick
- wechat
- wechatwork
- ccleaner
- slack
- google-chrome
- virtualbox
- vagrant
- raycast

cli package：

- warrensbox/tap/tfswitch(terraform 版本管理工具 https://github.com/warrensbox/terraform-switcher)
- jenv(java 版本管理工具 https://github.com/jenv/jenv)
- nvm(node 版本管理工具 https://github.com/nvm-sh/nvm)
- autojump(命令行强大的跳转工具 https://github.com/wting/autojump)
- kubectl(kubernetes 命令行工具 https://github.com/kubernetes/kubectl)
- zsh-autosuggestions(oh-my-zsh 自动提示插件 https://github.com/zsh-users/zsh-autosuggestions)
- zsh-syntax-highlighting(oh-my-zsh 高亮工具 https://github.com/zsh-users/zsh-syntax-highlighting)
- watch
- wget
- graphviz
- tmpwatch
- jq
- yq
- tmux
- go
- tree
- expect
- zsh
- openjdk
- colima
- docker
- docker-compose
- gnu-sed
- pyenv

如果上述软件不能满足需要，并且还想用 homebrew 安装，可以在下列两个数组中继续添加：

- cask: roles/homebrew/vars/main.yml > cask_list
- cli: roles/homebrew/vars/main.yml > cli_list

### git

配置 git alias.l = "log --graph --date=format:'%Y-%m-%d' --pretty=format:'%C(cyan)%h%Creset %Creset%C(auto)%d %s %C(black bold)(%ad) %C(bold blue)<%an>'"
