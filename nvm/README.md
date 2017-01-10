nvm(Node Version Manager) 是用于管理node的版本工具，可用来升级node

https://github.com/creationix/nvm  // 可以自己看 README.markdown 

// 若出现 $ 均表示为在命令行下输入, 没有 $ 也是在命令行下...

/*        安装          */

1) wget -qO- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash


/*       检查是否安装成功     */  // 貌似要另开一个terminal才行的样子orz...
command -v nvm  // 显示: nvm为成功
或
nvm --version   // 显示版本号为成功


/*        配置          */

按照官方 README.markdown 里 Install script 里的配置


或者如下：
// 参考 http://stackoverflow.com/questions/26476744/nvm-ls-remote-command-results-in-n-a 里的正确答案

$ nvm install node // $ 表示在命令行下输入

时出现： Version 'node' not found - try `nvm ls-remote` to browse available versions.

然后： $ nvm ls-remote 出现： N/A

在命令行下执行：
$ export NVM_NODEJS_ORG_MIRROR=http://nodejs.org/dist

再次执行： nvm ls-remote 出现： 一大堆node的版本号

最后:
$ nvm install node

显示如下：
Downloading and installing node v7.4.0...
Downloading http://nodejs.org/dist/v7.4.0/node-v7.4.0-linux-x64.tar.xz...
######################################################################## 100.0%
Computing checksum with sha256sum
Checksums matched!
Now using node v7.4.0 (npm v4.0.5)
Creating default alias: default -> node (-> v7.4.0)

$ node --version // => v7.4.0 成功:-)




