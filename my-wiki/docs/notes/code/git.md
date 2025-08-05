# git相关

## cmd命令
### **创建本地git仓库**
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
### **添加文件到git暂存区**
```
git add filename
# 或者添加所有修改的文件
git add .
```

### **将暂存区的更改提交到本地仓库，并添加提交信息：**
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

### **拉取**
```
git pull origin main
# 或者如果在新的分支上工作
git pull origin new-feature
```

### **推送**
```
git push origin new-feature
```
<div class="alert alert-warning" role="alert">
  先拉取(pull)再推送(push)!
</div>
    