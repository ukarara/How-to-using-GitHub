# git基本指令  
## 初始化  
* 打開terminal或cmd
* 設定使用者名稱與信箱
* 可以輸入  git config --list  可以查詢剛設定成功的名稱與信箱
```
$ git config --global user.name 
$ git config --global user.email 
```
## 新增檔案後
* git init :產生一個.git資料夾，並且讓git開始控制
* git status :查看被git控管的資料夾的狀態
* git remote add origin https://github.com/ukarara/sp109b
* git add
    - git add file.c :檔案交給站存區，並且讓Git開始追蹤這個檔案
    - git add *.txt :指定想加入的類型(.txt)
    - git add -A :追蹤全部
* git commit -m "簡短重要資訊" :把暫存區的檔案提交到倉庫裡面存檔
* git push origin branch :在現branch上把檔案push上去
* git log :查看先前的更改動作內容
* git clone :下載至本地
* git pull (origin branch) :把平台上更改的檔案更新下來
* git reset :檔案復原
    - git reset --soft :只有head重置到上一版
    - git reset --mixed :預設設定,將暫存區與head重置到上一版,工作目錄留下
    - git reset --hard :全部重置到上一版
## commit錯誤
1. 使用--amend修改  
`git commit --amend -m "修改的簡介" `

* 使用`git reset`復原
    - 先用gitlog查詢現在版本SHA值fb92aae
    - `git reset fb92aae~`或是~2、~3 或指定版本號
* git rebase :修改歷史

## 建立切換分支
* branch 分支 :相當於開分身,在不影響主工作狀態的情況下執行其他工作
* git branch main :新建分支"main"
* git branch : 知道有哪些main在branch中
* git checkout -b bugfix :建立一個新的Branch "bugfix" 並切換過去
* git checkout main: 切換分支(Switched to branch 'main')
* git merge bugfix :把我們的bugfix分支結合回去我們的main裡面
* git push origin main :就可以push剛剛整合好的main
* git branch -d bugfix :刪除bugfix分支  

## 建立.gitignore (未完成)
不想給別人看到的機密資訊
1. 後台的管理者帳號密碼
2. 重要文件


# 參考來源:
[30天教你學會Git](https://ithelp.ithome.com.tw/users/20129281/ironman/3348)
[https://git-scm.com/](https://git-scm.com/book/zh-tw/v2/%E9%96%8B%E5%A7%8B-%E5%88%9D%E6%AC%A1%E8%A8%AD%E5%AE%9A-Git)
