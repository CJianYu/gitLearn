# gitLearn
### 撤销git add

git reset HEAD .

### 修改commit信息

git commit --amend -m "an updated commit message"

### 撤销commit

git reset --soft HEAD^   （HEAD^的意思是上一个版本，也可以写成HEAD~1，如果你进行了2次commit，想都撤回，可以使用HEAD~2）

### vim模式编辑 

那如何操作vim编辑器(这里只简单介绍 一下)：

1. 按下字母键`i`或`a`或`o`，此时进入到可编辑状态，这时就可以输入你的注释
2. 当你输入完之后，按下`Esc`键就可退出编辑状态，回到一般模式。
3. 最后就是怎么退出vim编辑器并提交commit， 有两种方法：
   - 输入两字大写字母`ZZ`（记住是大写）
   - 输入`:wq`或`:wq!`(强行退出)

### 某仓库更改用户名邮箱

git config user.name "gitlab's Name"

git config user.email "gitlab@xx.com"

git config --list

### 上线后的项目修改

方法一：

切换到master分支，新建一个分支

将开发分支的修改提交cherry-pick过来

方法二：

切换到master分支，新建一个分支，直接在新分支改

