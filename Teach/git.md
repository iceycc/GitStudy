###    git入门与实践
- 版本控制工具：
    >集中式管理 （svn）
    >分布式管理（git）




## 基础操作


### 3个区 

工作区,暂存区，仓库

### 4种状态


- Untracked （未跟踪）
> 文件没有被添加到暂存区，也没有被提交过! 

- Unmodify (未修改)
> 自从上次提交后没有改过代码(提交之后，没有修改过代码，那么这个代码就是Unmodify状态)

- Modified (已修改)
>  自从上一次提交后，修改了文件的内容,那么文件的状态就会变为Modified

- Staged （暂存状态）
> 一旦，我把文件添加到暂区，那么这个文件的状态就变为了Staged


## 配置git (一个电脑只要配置一次)
配置用户名和邮箱:
输入命令: 
配置用户名: `git config --global user.name "自己的名字"`
配置邮箱: `git config --global user.email "自己的邮箱"`
>补充，其实是保存了用户名和邮箱到 C:\Users\[用户名]\.gitconfig文件中
>git init 初始化仓库


####  写代码步奏


- 配置用户信息(全局用户名)
   > git config --global user.name '用户名'
   > git config --global user.email '邮箱'

-  创建仓库
   > git init

- 查看仓库状态
   > git status

- 追踪文件
   > git add 文件名

- 提交: 将文件备份到仓库中
   > git commit -m '提交信息'

- 查看备份的日志
   > git log

- 如果更改了文件
   > 凡是修改了文件都需要 add 一下, 再 commit

- 返回到指定版本
   > git reset --hard SHA1值

- 从库中删除    


   - $ git checkout -- test.txt	

- 恢复从库中误删的文件


   - $ git checkout -- test.txt

#### 常用的命令行

- > cd 改变目录
- > pwd 改变工作目录
- > mkdir 新建文件夹
- > touch 新建文件
- > rmdir 删除文件夹
- > rm -rf 删除文件
- > ls 查看文件列表
