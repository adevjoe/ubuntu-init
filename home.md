
### 首先设置软件源

系统设置 -> 软件和更新 -> 下载至  改为 http://mirrors.aliyun.com/ubuntu

```bash
cp /etc/apt/sources.list /etc/apt/sources.list.bak
# 修改为阿里云的镜像源
cat > /etc/apt/sources.list << END
deb http://mirrors.aliyun.com/ubuntu/ xenial-security main restricted
# deb-src http://security.ubuntu.com/ubuntu xenial-security main restricted
deb http://mirrors.aliyun.com/ubuntu/ xenial-security universe
# deb-src http://security.ubuntu.com/ubuntu xenial-security universe
deb http://mirrors.aliyun.com/ubuntu/ xenial-security multiverse
# deb-src http://security.ubuntu.com/ubuntu xenial-security multiverse
END

# 更新源列表信息
apt-get update
```



### 更新
````
sudo apt-get update
````

### shadowsocks-qt5
````
sudo add-apt-repository ppa:hzwhuang/ss-qt5
sudo apt-get update
sudo apt-get install shadowsocks-qt5
````

### chrome
````
sudo wget http://www.linuxidc.com/files/repo/google-chrome.list -P /etc/apt/sources.list.d/
wget -q -O - https://dl.google.com/linux/linux_signing_key.pub  | sudo apt-key add -
sudo apt-get update
sudo apt-get install google-chrome-stable
````

### vim(+推荐插件)
````
sudo apt-get install vim
wget -qO- https://raw.github.com/ma6174/vim/master/setup.sh | sh -x
````

### indicator-sysmonitor(实时系统信息显示)
````
sudo add-apt-repository ppa:fossfreedom/indicator-sysmonitor
sudo apt-get update
sudo apt-get install indicator-sysmonitor
````

### java
````
sudo add-apt-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java8-installer
````

### node
````
sudo apt-get install nodejs-legacy
sudo apt-get install npm
sudo npm install -g nrm --registry=https://registry.npm.taobao.org
nrm use taobao
sudo npm install npm@latest -g
sudo npm install -g n
sudo n latest
````

### albert
````
sudo add-apt-repository ppa:nilarimogard/webupd8
sudo apt-get update
sudo apt-get install albert
````
### 搜狗输入法
```
http://pinyin.sogou.com/linux/
```

### terminator+ on-my-zsh +autojump
```
// 安装terminator
sudo apt-get install terminator


// 安装zsh：

sudo apt-get install zsh安装zsh
zsh --version确认是否安装成功
sudo chsh -s $(which zsh)设置zsh为默认shell
注销重新登录

//安装Oh-My-Zsh
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

// 安装autojump
git clone git://github.com/joelthelion/autojump.git
cd autojump
./install.sh
复制提示的信息到.zshrc
source .zshrc

```

### systemback
```
sudo add-apt-repository ppa:nemh/systemback
sudo apt-get update
sudo apt-get install systemback
```

### playonlinux
````
wget -q "http://deb.playonlinux.com/public.gpg" -O- | sudo apt-key add -
sudo wget http://deb.playonlinux.com/playonlinux_trusty.list -O /etc/apt/sources.list.d/playonlinux.list
sudo apt-get update
sudo apt-get install playonlinux
````
### 娱乐软件

- 视频播放器 SMPlayer
