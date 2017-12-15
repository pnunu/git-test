
上传 
```
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/pnunu/git-test.git
git push -u origin master
```

…or push an existing repository from the command line

```
git remote add origin https://github.com/pnunu/git-test.git
git push -u origin master
```

# 取得Git仓库

1、 初始化一个版本仓库 

``` git init ```

2、 Clone远程版本库

``` git clone yourgitaddress(你的git地址) ```

3、 添加远程版本库origin

``` git remote add origin yourgitaddress(你的git地址) ```

4、 查看远程仓库

``` git remote -v ```

# 提交你的修改

1、 添加当前修改的文件到暂存区

``` git add . ``` 

2、 如果你自动追踪文件，包括你已经手动删除的，状态为Deleted的文件

``` git add -u ``` 

3、 提交你的修改

``` git commit –m "你的注释" ``` 

4、 推送你的更新到远程服务器,语法为 git push [远程名] [本地分支]:[远程分支]

``` git push origin master ``` 

5、 查看文件状态

```  git status ``` 

6、 跟踪新文件

``` git add readme.txt ``` 

7、 从当前跟踪列表移除文件，并完全删除

``` git rm readme.txt ``` 

8、 仅在暂存区删除，保留文件在当前目录，不再跟踪

``` git rm –cached readme.txt ``` 

9、 重命名文件

``` git mv reademe.txt readme ``` 

10、 查看提交的历史记录

``` git log ``` 

11、 修改最后一次提交注释的，利用–amend参数

``` git checkout –- readme.txt ``` 


# 基本的分支管理

1、 创建一个分支

``` git branch workspace ``` 

2、 切换工作目录到workspace

``` git chekcout workspace ``` 

3、 将上面的命令合在一起，创建workspace分支并切换到workspace

``` git chekcout –b workspace ``` 

4、 合并workspace分支，当前工作目录为master

``` git merge workspace ``` 

5、 合并完成后，没有出现冲突，删除workspace分支

``` git branch –d workspace ``` 

6、 拉去远程仓库的数据，语法为 git fetch [remote-name]

``` git fetch ``` 

7、 fetch 会拉去最新的远程仓库数据，但不会自动到当前目录下，要自动合并

``` git pull ``` 

8、 查看远程仓库的信息

``` git remote show origin ``` 
