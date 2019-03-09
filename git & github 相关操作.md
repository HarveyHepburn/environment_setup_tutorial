# 生成SSH key

```
ssh-keygen -t rsa -C"lincheung0@gmail.com"
```
# 初始化git仓库

```
git init
```
# 从远程克隆一个git仓库

```
git clone git@github.com:LinCheungS/python_tiny_project.git
```
# 添加远程仓库为上传仓库

```
git remote add origin git@github.com:LinCheungS/python_tiny_project.git
```

# 增加 确认提交 上传 

```
git add -A

git commit -m "注释"

git push

```

# 关于branch操作
```
# 新建branch
git branch new_branch

# 切换到新的branch
git checkout new_branch
```
# 常用mac简化
```
alias gs="git status"
alias gc="git commit -m "
alias ga="git add -A"
alias gp="git push"
```


