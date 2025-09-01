# git相关

## cmd命令

---

### 命令速查
初始化和配置
```
git init：初始化一个新的 Git 仓库。
git config --global user.name "Your Name"：设置全局用户名。
git config --global user.email "your.email@example.com"：设置全局用户邮箱。
```
工作区和暂存区操作
```
git status：查看工作区状态，包括已跟踪和未跟踪的文件。
git add <file>：将文件添加到暂存区。
git add .：将所有更改（包括新文件、修改过的文件、删除的文件）添加到暂存区。
git rm <file>：删除工作区中的文件，并从暂存区移除。
git mv <old-file> <new-file>：移动或重命名文件，并更新暂存区。
```
创建新分支
```
git branch <branch-name>        #创建一个新分支，但不切换到该分支。
git checkout -b <branch-name>   #创建一个新分支，并立即切换到该分支。
```
查看分支
```
git branch      # 查看分支
git branch -r   # 列出所有远程分支。
git branch -a   #列出所有本地和远程分支
```
删除分支
```
git branch -d <branch-name>：删除一个已经完全合并到当前分支的本地分支。
git branch -D <branch-name>：强制删除一个本地分支，不管它是否已经合并。
```
设置跟踪关系
```
git branch -u <remote>/<branch>
或 git branch --set-upstream-to <remote>/<branch>：为当前分支设置上游（跟踪）分支。
git branch --set-upstream <branch> <remote>/<branch>：为指定的本地分支设置上游分支。
```
重命名分支
```
git branch -m <old-branch-name> <new-branch-name>：重命名当前分支。
git branch -m <old-branch-name> <new-branch-name>：重命名指定的本地分支。
```
合并分支
```
git merge <branch-name>：将指定的分支合并到当前分支。
```
提交更改
```
git commit -m "Commit message"：提交暂存区的更改。
git commit -a：提交所有已跟踪文件的更改（跳过暂存区）。
git commit --amend：修改上一次提交（例如，修改提交信息）。
```
远程仓库操作
```
git remote add origin <remote-repo-url>：添加远程仓库。
git remote -v：查看远程仓库的 URL。
git fetch <remote>：从远程仓库获取最新的更改。
git pull <remote> <branch>：从远程分支拉取更改并合并到当前分支。
git push <remote> <branch>：将本地分支推送到远程仓库。
git push <remote> --delete <branch>：从远程仓库删除一个分支。
```
查看历史和日志
```
git log：查看提交历史。
git log --oneline：以简洁格式查看提交历史。
git log <commit>：查看特定提交的详细信息。
git blame <file>：查看文件中每一行的最后修改者。
```
撤销操作
```
git reset <file>：将文件从暂存区移除。
git checkout -- <file>：将文件恢复到上一次提交的状态。
git revert <commit>：创建一个新的提交，撤销指定提交的更改。
git reset --hard：将工作区和暂存区都恢复到上一次提交的状态（危险操作，会丢失未提交的更改）。
```
标签管理
```
git tag <tag-name>：创建一个轻量级标签。
git tag -a <tag-name> -m "Tag message"：创建一个带注释的标签。
git push <remote> <tag-name>：将标签推送到远程仓库。
```

---

### 个人笔记
#### **创建本地git仓库**
```
git init
# 也可以指定仓库目录
git init newrepo
```
该命令执行完后会在当前目录生成一个 .git 目录。  
或者克隆一个仓库
```
git clone
```
#### **添加文件到git暂存区**
```
git add filename
# 或者添加所有修改的文件
git add .
```

#### **将暂存区的更改提交到本地仓库，并添加提交信息：**
```
git commit -m "Add new feature"
```
常见提交类型

* `init`- 初始化项目
* `feat`- 新功能
* `fix`- 修复bug
* `docs`- 文档变更
* `style`- 代码风格变动
* `refactor`- 代码重构
* `perf`- 性能优化
* `test`- 添加或修改测试
* `chore`- 杂项
* `build`- 构建系统或外部依赖项的变更
* `ci` 持续集成配置的变更
* `revert`- 回滚

#### **拉取**
```
git pull origin main
# 或者如果在新的分支上工作
git pull origin new-feature
```

#### **推送**
```
git push origin new-feature
```
<div class="alert alert-warning" role="alert">
  先拉取(pull)再推送(push)!
</div>

#### **分支操作**

---

### 关于提交撤回`一般不撤回`
如果已经push
```
git checkout -b feature/my-fix  # 基于当前分支的代码创建新分支
git checkout main               # 回到已经提交的main分支
git fetch upstream              # 将上游仓库的所有分支、提交全部拉到本地，但不合并，也不改任何本地分支。
git reset --hard upstream/main  # 本地 main 回退
git push -f origin main         # 强制推，覆盖远程 main
```
如果还未push
```
git checkout -b feature/my-fix   # 创建并切换
# 改动已自动带过来
git push -u origin feature/my-fix   # push新分支
git checkout main                   # 回到main分支
git fetch upstream                  # 同上
git reset --hard upstream/main      # 本地彻底回退
git push -f origin main             # 强制同步回你的 fork
```