# vision control system

## prepare

1.  git --version

2.  touch file

3. mkdir folder

4.  cd（ change directory）
    1.  cd   ..上一级
    2.  cd    . 没变
    3.  cd    c:
    
5. ~ (root)
6. exit 退出
7. clear 清屏

## config
1.  git  config  --help(link)
2.  git congfig -h
1.  git  config --global use.name 'jack'
2.  git  config --global user.email '@xx.com'
3.  git config user.name  or  user.email
## begin
1. git init
2. ls -a (隐藏)
3. e.g. touch 1.py
4. git  status   /   git status  -s(简略)
2. git  add 1.py  

   1.   git add .  
6. git  commit  -m   "描述”
## log
7. git log  (日志)  / git log --oneline    / git log --oneline --reverse  (展示的是commit)
8. pwd : print working directory（当前所在文件夹)
6. git diff  unstaged
## diff
1. git diff --cached 查看 all 已经暂存起来的状态，（ --staged 和 --cached 是同义词）
2. git commit --amend  --no-edit（后面的no是保证描述不变，amend在add后执行  但是提交到最新的chance中， 没有增加新的log  amend后面可以增加描述信息
## RESET
12. e.g git reset 1.py    (add之后使用  返回暂存区)
13. git reset --hard HEAD  ()
14. git reset --hard head~2(index从0开始) --hard 3747a40 
15. git reflog 
16. git reset --hard 3747a40   / --hard HEAD@{1}  
17. git  checkout 14f221b  --  1.py  (git  log 显示的描述信息还是以前的  )

## brand 

1. git log --oneline  --graph 展示节点图  （有*）
2. 建立分支
   1.  git branch  name
   2. git checkout -b name (建立分支  and  跳到该分支上)
   3. git  branch  查看在哪一个branch上  *就是
   4. gir check name  选择分支
   5. git branch -d   name    delete  分支 (删除某一个分支  本身不能在那个分支上)
   6. git  commit -am"description  news”（前提不是news  file  必须是已经在Repo）\
## brand conflict
   7. git merge --no-ff -m "t"  oops     （ff  是fast-forward  ，no是为了在log上显示merge信息    默认是看不到信息的)
   8. git  merge oops
   9. git rebase oops  
   10.  git add 1.py
   11. git rebase --continue(前后rebase后的id不一样   rebase后 的所在分支是平行时空）没有历史版本
## 临时托管
   12. ) git stash（即使未add也没关系  临时有新duty最好开新branch）
   13.  git stash  pop
   14. vim  保存就是enter  eac ZZ

## 上传

1. git remote add origin http://
2. git push -u  origin master(branch  name)
3. history  （看commit记录）
4. .git 也会被上传
5. 本地repo和remote  可以不一样



![image-20210617001837447](C:\Users\卡布奇诺\AppData\Roaming\Typora\typora-user-images\image-20210617001837447.png)

