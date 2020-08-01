# Learn Git
Git管理文件的三大部分：工作区，暂存区，仓库

工作区：工作目录，文件的原始位置

暂存区：暂存修改后的文件

仓库：保存最终版本库中的文件



## 常用流程

修改文件后，将修改记录保存在暂存区中，并提交至版本库

- git add filename1

文件1从工作区>>>>暂存区



- git commit -m “修改记录”

文件从暂存区>>>>仓库





## 查看文件自上次add或commit之后修改的部分

- git diff

比较工作区和暂存区的差异



- git diff —cached

比较暂存区和仓库的差异



- git diff HEAD

比较工作区和仓库的差异



## 回退文件

- git checkout -- filename.txt

文件从暂存区>>>>工作区



- git reset HEAD

文件从仓库>>>>暂存区



- git restore –worktree filename.txt

文件从工作区删除