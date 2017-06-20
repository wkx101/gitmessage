# 使用git commit模板
如何使用打造細緻的git commit，我不擅長與人溝通，所以很多情況都會跳句子，而這個強迫內容詳細化，應該是符合我想要的。

## 5W1H的應用
- who (誰)
- when (何時)
- where (哪裡)
- what (幹啥)
- why (為何)
- how (怎做)
基本上git commit就已經有who、when、where的存在，所以我只需要紀錄剩下的what、why、how
1. **what** 以主題式一行帶過
2. **why** 為什麼要這樣做
3. **how** 實際上做了甚麼

## 模板的應用
隨意建立一個檔案作為模板，這邊我所建立的檔案是.gitmessage，然後我拿去放的.gitconfig的旁邊，至於.gitconfig在哪裡？請自行尋找(win系列大概在user裏頭)

這邊的重點是別忘記配置到.gitconfig裏頭去，作法如下
```
[commit]
  template = ~/.gitmessage
```
或者直接輸入指令
```
git config --global commit.template "~/.gitmessage"
```
