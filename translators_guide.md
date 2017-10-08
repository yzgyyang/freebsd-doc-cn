# 翻译指南 Translator's Guide

## 新译者 New Contributor

完成首次设置后，提交一个 Pull Request 将自己加入 [README.md](README.md) 中的 `贡献者` 列表中。

## 首次设置 Init

安装相关依赖:  

- `git`
- 一种 PO 编辑器 (例如 `Poedit` [Poedit 下载](https://poedit.net/))

Git设置:

- 将 https://github.com/yzgyyang/freebsd-doc-cn fork 到自己的 Github。

- 将自己 fork 过来的 repo clone 到本地:  
`git clone https://github.com/your-username-here/freebsd-doc-cn`

- 进入项目文件夹:
`cd freebsd-doc-cn`

- 设置上游跟踪 repo:  
`git remote add upstream https://github.com/yzgyyang/freebsd-doc-cn`

- 检查是否成功设置了上游:  
`git remote -v`  
期望的输出:
```
origin    https://github.com/your-username-here/freebsd-doc-cn (fetch)
origin    https://github.com/your-username-here/freebsd-doc-cn (push)
upstream  https://github.com/yzgyyang/freebsd-doc-cn (fetch)
upstream  https://github.com/yzgyyang/freebsd-doc-cn (push)
```

## 翻译流程 Workflow

- 和 ygy 联系分配任务，并更新状态。

- 从上游拉取最新数据:  
`git pull --rebase upstream master`  
*若本地没有未保存的更改，而 rebase 出现了错误，可以尝试强制更新 repo:*  
`git fetch upstream master`  
`git reset --hard upstream/master`

- 使用一种 PO 编辑器 (例如 `Poedit` [Poedit 下载](https://poedit.net/)) 对认领部分进行翻译:  
`poedit zh_CN.po`

- Commit:  
`git add zh_CN.po`  
`git commit -m "Update XXX"`

- 翻译完成后，向上游提交 Pull Request，并 @yzgyyang 进行 review。
