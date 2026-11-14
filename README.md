# git 练习仓库

用来练手的 Git 仓库，记录常用命令和操作笔记。

## 常用命令速查

### 初始化与提交

```bash
git init                      # 把当前文件夹变成仓库
git status                    # 看当前状态（最常用）
git add .                     # 把所有改动加入暂存区
git add 文件名                # 只加某个文件
git commit -m "说明"          # 提交到本地
git log --oneline             # 看提交历史
```

### 推送到 GitHub

```bash
git remote add origin https://github.com/tingtian641102/git.git   # 关联远程（只需一次）
git push -u origin main       # 首次推送并建立追踪
git push                      # 之后直接推
git pull                      # 拉取远程更新
```

### 分支

```bash
git branch                    # 列出分支
git switch -c 新分支名        # 新建并切换
git switch main               # 切回 main
git merge 分支名              # 合并某分支到当前分支
```

### 撤销与回退

```bash
git restore 文件名            # 丢弃工作区的改动
git restore --staged 文件名   # 从暂存区撤回
git reset --soft HEAD~1       # 撤销最近一次提交，保留改动
```

## 三条最该记住的原则

1. **提交前先 `git status`**，看清自己要提交什么。
2. **一次提交只做一件事**，说明写清楚做了什么。
3. **推之前先 `git pull`**，避免远程有更新导致冲突。
