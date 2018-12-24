## blog

地址：[https://small-teenager.github.io/](https://small-teenager.github.io/)
## Github pages + aircloud
this is my blog.

## hexo在GitHub上搭建个人博客过程
以aircloud 为例

github 项目repo name：name.github.io    name为github上的名字 不可更改

### 环境搭建

安装node.js 和git

安装完成后进入命令行 输入 node -v,  npm -v, git -version 查看信息

### SSH 授权
打开git bash 输入ssh-keygen -t rsa 回车3次
 
打开C 盘用户目录下.shh文件夹下，用记事本打开id_rsa.pub 复制其中的内容添加到GitHub上

id_rsa 密钥
id_rsa.pub 公钥

### SSH 测试
打开 git bash 输入ssh -T git@github.com

返回Hi username ！You've successfully ......说明你已经成功啦！

### 设置本地博客的配置

#### 安装hexo

在任意一个地方新建一个文件夹，在git bash中进入这个文件夹，比如cd /d/blog（之后安装的内容会保存在这个文件夹内），
输入npm install -g hexo安装hexo

npm install hexo --save

hexo v  查看是否安装成功

#### 初始化hexo
hexo init 初始化
hexo s 启动服务

####　更改主题
在git hash 命令窗口下 ，进入／themes 下载主题，输入git clone url

修改 _config.yml   

## 上传到github
hexo g

hexo d

## hexo 添加站内搜索
npm i hexo-generator-search --save

## 赞未加评论功能