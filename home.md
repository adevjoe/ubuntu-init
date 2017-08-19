
### 首先设置软件源

系统设置 -> 软件和更新 -> 下载至  改为 http://mirrors.aliyun.com/ubuntu

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
