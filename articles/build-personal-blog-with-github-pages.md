#利用github创建个人博客的两种方式：
参见官方说明[github pages](https://help.github.com/articles/user-organization-and-project-pages 'github pages')

##一.利用project pages创建个人博客

1. 在github创建仓库，例如blog
2. 在本机搭建博客目录及内容，例如目录blog
3. 在本地目录blog中git init
4. 使用语句git checkout --orphan gh-pages创建,gh-pages分支内容作为网站内容
5. 发布内容，将分支内容发布到远程仓库blog中，具体步骤如下：
	1. 添加所有内容至版本控制git add .
	2. 提交内容到本地仓库git commit -m 'commit my blog'
	3. 关联远程仓库git remote add origin git@github.com:caochao/blog.git
	4. 推送本地内容至远程仓库git push -u origin gh-pages
6. 访问博客http://caochao.github.com/blog/

##二.利用usr/organization pages创建个人博客
1. 在github上创建名为caochao.github.com的仓库
2. master分支内容作为网站内容
3. 访问博客http://caochao.github.com