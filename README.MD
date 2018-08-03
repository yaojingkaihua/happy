git使用笔记
-------------
* 打开bit bash
* 进入D盘

        cd /d

* 建立git文件夹

        mkdir git

* 进入git文件夹

        cd git

* 建立github文件夹

        mkdir github

* 进入github文件夹

        cd github

* 显示当前文件夹

        pwd

  * 当前路径显示/d/git/github,建立完文件夹之后可以用下面代码进入路径

            cd /d/git/github

* 克隆项目（需要先在github建立仓库Repository）
        
        git clone https://github.com/yaojingkaihua/happy.git

* 添加文件到d:/git/github目录下，查询git状态

        git status

    *<span style='color:red'>红色</span>表示新文件或者修改的文件没有被追踪版本*

* 把文件加入的git版本追踪系统（只是给文件加了个index索引）

        git add <git status显示的文件名>

* 查看状态

        git status

    *<span style='color:green'>绿色</span>表示新文件或者修改的文件已被追踪版本，但还没提交到本地库*

* 提交到本地版本库

        git commit -m "<提交说明>"

* 查看状态

        git status
        显示>nothing to commit, working tree clean

    *nothing to commit, working tree clean表示工作区没有修改，都提交到了本地

* 提交到远程版本库

        git push origin happy

    *origin是你的远程仓库，happy是分支，可以根据需要替换，你的项目可以关联多个仓库和多个分支，如果提交默认的就下面简写就够了*

            git push

* 查看提交历史

            git log [-p] [--all][--stat]

    + -p显示详细修改内容
    + --all显示全部分支的提交历史
    + --stat显示修改统计
     
