#test git fetch

#no-ff merge

#create new dev

#2019.5.4

# github_tutorials

新电脑设置用户名和邮箱：

git config --global user.name "Your Name"

例：git config --global user.name "ZGD"

git config --global user.email "email@example.com"

例：git config --global user.email "342167339@qq.com"

创建ssh密钥：

ssh-keygen -t rsa -C "youremail@example.com"

例：ssh-keygen -t rsa -C 342167339@qq.com

然后将～/.ssh中的id_rsa.pub公钥添加到github中

最后在github上添加仓库，记得不要自动生成README.md文件

----以下步骤在生成一个新仓库后github会给出提示----

初始化需要同步的文件夹：

git init

添加远程仓库：

git remote add origin git@github.com:342167339/learngit.git  #origin为远程仓库在本机的名字，一般为origin，后面为github仓库

第一次推送master分支的所有内容：

git push -u origin master

添加文件修改到缓存区

git add <file>，注意，可反复多次使用，添加多个文件

将文件删除修改到缓存区

git rm <file>

提交缓存区修改到本地仓库

git commit -m "一定要添加修改说明"

git commit -a # 提交所有修改

推送最新修改：

git push origin master
