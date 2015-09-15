<https://github.com/blog/broadcasts>

Read [Jekyll Quick Start](http://jekyllbootstrap.com/usage/jekyll-quick-start.html)

Complete usage and documentation available at: [Jekyll Bootstrap](http://jekyllbootstrap.com)

<http://www.ruanyifeng.com/blog/2012/08/blogging_with_jekyll.html>
<http://blog.csdn.net/on_1y/article/details/19259435>

### 三分钟建立Github博客

Reference:<http://jingyan.baidu.com/article/6fb756eca39760241858fbca.html>

1. 建立一个新的Gibhub代码库到https://github.com建一个新的代码库，名字必须为username.github.io，其中username为你的gibhub用户名。

2. 安装Install Jekyll-Bootstrap进入shell，输入下面代码：
$ git clone https://github.com/plusjade/jekyll-bootstrap.git USERNAME.github.io
$ cd USERNAME.github.io
$ git remote set-url origin git@github.com:USERNAME/USERNAME.github.io.git
$ git push origin master

3. 完成等待几分钟，这段时间里面github会自动编译你的上传，然后在浏览器里面打开username.github.com，你的Github就魔法般的出现了。

---
### 安装jekyll
$ gem install jekyll
ERROR:  Could not find a valid gem 'jekyll' (>= 0), here is why:
          Unable to download data from https://rubygems.org/ - Errno::ECONNRESET: An existing connection was forcibly closed by the remote host. - SSL_connect (https://rubygems.org/latest_specs.4.8.gz)

Reference:<http://www.th7.cn/system/lin/201503/97354.shtml>

kxw@KINGSON_WU /f/kingson4wu.github.io (master)
$ gem sources -a http://ruby.taobao.org/
http://ruby.taobao.org/ added to sources###

---
### Run Jekyll Locally
1. $ cd USERNAME.github.com
2. $ jekyll serve

>Configuration file: f:/kingson4wu.github.io/\_config.yml<br />
Source: f:/kingson4wu.github.io<br />
Destination: f:/kingson4wu.github.io/\_site<br />
Generating..  done.
Please add the following to your Gemfile to avoid polling for changes: gem 'wdm', '>= 0.1.0' if Gem.win_platform?<br />
Auto-regeneration: enabled for 'f:/kingson4wu.github.io'<br />
Configuration file: f:/kingson4wu.github.io/\_config.yml<br />
Server address: http://127.0.0.1:4000/<br />
Server running... press ctrl-c to stop.<br />
Regenerating: 1 file(s) changed at 2015-09-14 23:26:26 ...done in 0.43529 seconds.

---
###  Create a Post
Create posts easily via rake task:

$ rake post title="Hello World"
>Creating new post: ./\_posts/2015-09-14-hello-world.md<br />


---
### Create a Page

1. Create pages easily via rake task:<br />
$ rake page name="about.md"
>mkdir -p .<br />
Creating new page: ./about.md

2. Create a nested page:<br />
$ rake page name="pages/about.md"
>mkdir -p ./pages<br />
Creating new page: ./pages/about.md

3. Create a page with a "pretty" path:<br />
$ rake page name="pages/about"
>mkdir -p ./pages/about<br />
Creating new page: ./pages/about/index.html

### Publish
After you've added posts or made changes to your theme or other files, simply commit them to your git repo and push the commits up to GitHub.

1. $ git add .
2. $ git commit -m "Add new content"
3. $ git push origin master


<http://jekyllbootstrap.com/usage/jekyll-quick-start.html>

### Using Themes

1. $ rake theme:install git="https://github.com/jekyllbootstrap/theme-the-program.git"
2. $ rake theme:install name="THEME-NAME"
3. $ rake theme:switch name="the-program"
