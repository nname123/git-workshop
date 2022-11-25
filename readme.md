## 上課心得
上完這堂課讓我更加理解Git的用法，我自己覺得上次講Git的老師講的就沒那麼清楚，現在對於工作目錄、暫存區、儲存庫這三個存檔位置有更加理解，但我還是有一些小問題。

## 畫格子
| 工作目錄  | 暫存區 |儲存庫|
| ------------- |:---------------------:|--------------------|
| 正在編輯的檔案| git add 之後的儲存位置|git commit之後的位置|

## 小問題
原本對於Github下載資料的方法有疑問，現在已大致理解沒問題了，順便紀錄一下。
## 第一次上傳

commit完後用下面的指令建立與遠端的連線
```
git remote add origin {url}
```
url有分`https`跟`ssh`   
>`ssh`上傳時不用輸入帳密,但需要先在電腦設定ssh且Github帳號要輸入ssh公鑰認證   

>`https`上傳時需輸入帳密登入Github

之後用這兩個老師講過的指令
```
git branch -M main
git push -u origin main
```
之後就可以正常編輯push/pull


## Github上已經有檔案時

用clone指令下載到電腦

```
git clone {url}
```
然後要進去clone下來的資料夾
```
cd {clone下來的資料夾}
```
之後就可以正常編輯push/pull








