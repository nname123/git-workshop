## 上課心得
上完這堂課讓我更加理解Git的用法，我自己覺得上次講Git的老師講的就沒那麼清楚，現在對於工作目錄、暫存區、儲存庫這三個存檔位置有更加理解，但我還是有一些小問題。

## 畫格子
| 工作目錄  | 暫存區 |儲存庫|
| ------------- |:---------------------:|--------------------|
| 正在編輯的檔案| git add 之後的儲存位置|git commit之後的位置|

## 小問題
我把家裡電腦想要用git pull 上課資料回電腦的時候，發現一些奇怪的問題，
之前的老師有教我麼使用ssh連線，那我在家想用ssh連線有需要那個ssh檔案嗎?還是說輸入密碼就能Push/Pull呢?

我記得要連線遠端是要用三個指令，我在家使用這個指令之後他報錯
```
git remote add origin {url}
```
結果顯示
`error: remote origin already exists.`  
看起來是檔案已存在，我google一下之後使用
```
git remote rm origin 
```
之後再試就可以了。我看了一下應該是刪除origin這東東再新增就不會錯誤，因為是刪除所以我檢查了github上的檔案好像也沒東西不見，之後google發現
>origin 表示遠端，master 表示分支名，接在 origin 之後表示是遠端分支名。

我對這部分有點混亂，課堂上有把 master 改成 main，然後又分遠端跟本地端
* master：本地分支名。
* origin master：origin 表示遠端，master 表示分支名，接在 origin 之後表示是遠端分支名。
* origin/master：遠端分支在本地的拷貝，因此稱為本地分支。

看起來我刪掉的origin是遠端上的連結?我在家改了之後不知道之後用教室的電腦會不會報錯...
不太了解不同設備要對同一份git編輯上傳的具體步驟是什麼，老師有示範首次上傳的方法，那第二台設備的連結方式也是一樣那三個指令嗎?







