## 安装

``` bash
# 解压
tar xzvf node-v4.6.1.tar.gz

# 进入到解压后的文件夹
cd node-v4.6.1 // 

./configure

make

# 要用管理员权限，如sudo make install等
make install
```


## 修改配置

``` bash
# 修改源
npm config set registry https://registry.npm.taobao.org

# 验证是否成功
npm config get registry
```


## 升级npm

``` bash
# 管理员权限下
npm install npm -g


## 升级node.js
**用nvm**


