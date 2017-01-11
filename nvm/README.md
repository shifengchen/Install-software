## nvm(Node Version Manager)

**用于管理node的版本工具，可用来升级node**

**https://github.com/creationix/nvm  // 可以自己看 README.markdown **

## 安装

``` bash
wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash
```


## 检查是否安装成功

**貌似要另开一个terminal才行的样子orz...**

``` bash
# 输出 nvm 为成功
command -v nvm

# 或

# 显示版本号为成功
nvm --version
```


## 配置

**可按照官方 README.markdown 里 Install script 里的配置**

> `nvm install node` 时出现： Version 'node' not found - try `nvm ls-remote` to browse available versions.

``` bash
# 显示： N/A
nvm ls-remote
```

**解决方法**
``` bash
export NVM_NODEJS_ORG_MIRROR=http://nodejs.org/dist

# 将显示一大堆node的版本号
nvm ls-remote

$ nvm install node

# 显示如下：
# Downloading and installing node v7.4.0...
# Downloading http://nodejs.org/dist/v7.4.0/node-v7.4.0-linux-x64.tar.xz...
# ######################################################################## 100.0%
# Computing checksum with sha256sum
# Checksums matched!
# Now using node v7.4.0 (npm v4.0.5)
# Creating default alias: default -> node (-> v7.4.0)

# 显示如：v7.4.0 则为成功:-)
node --version
```

**参考 http://stackoverflow.com/questions/26476744/nvm-ls-remote-command-results-in-n-a 里的正确答案**




