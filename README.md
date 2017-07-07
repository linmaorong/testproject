# GIT 的安装到链接到github(git自己服务器搭建比较麻烦 暂不做介绍)
# 安装地址新手教程 http://www.runoob.com/git/git-install-setup.html
# 链接github  
# 注册github新手教程 http://www.runoob.com/git/git-remote-repo.html
# git与github之间的传输是通过SSH加密的，所以第一步先在本地生成一.ssh
# 1. 先查看本地是否有.ssh文件，有的话删掉　　cd ~/.ssh
  2. ssh-keygen -t rsa -C "your email@.com"
  3. 这样就表示成功了，会在C盘的 用户目录的根目录下生成一个.ssh文件，如果找不到，可以搜索一下，文件下会有id_rsa与id_rsa.pug俩个文件
  4. ssh -t git@github.com 检测是否链接成功
  5. 上传项目
     在终端找到自己的项目
     git init
     git add .
     git commit -m "fist commit"
     git remote add origin git@github.com:linmaorong/myvue.git  (linmaorong是你注册github账号是使用的名字 myvue是在github上新建项目是使用的名字 推荐跟你自己要上传的项目名字保持一致 可能会报错fatal:remote origin already exists) 如果不报错 执行下一步
     解决办法 先输入： git remote rm origin  再输入： git remote add origin git@github.com:linmaorong/myvue.git  
     git push -u origin master

     恭喜您 您的项目已经成功上传到github了！
