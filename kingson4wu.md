### 三分钟建立Github博客

Reference:<http://jingyan.baidu.com/article/6fb756eca39760241858fbca.html>

1. 建立一个新的Gibhub代码库到https://github.com建一个新的代码库，名字必须为username.github.io，其中username为你的gibhub用户名。

2. 安装Install Jekyll-Bootstrap进入shell，输入下面代码：
$ git clone https://github.com/plusjade/jekyll-bootstrap.git USERNAME.github.io
$ cd USERNAME.github.io
$ git remote set-url origin git@github.com:USERNAME/USERNAME.github.io.git
$ git push origin master

3. 完成等待几分钟，这段时间里面github会自动编译你的上传，然后在浏览器里面打开username.github.com，你的Github就魔法般的出现了。
