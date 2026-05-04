# 第九週加分作業：Tool Calling

## 一、工具內容

本次使用的工具為 Hermes Agent 的 terminal / commands 工具。

這個工具可以讓 Agent 在本機電腦中執行終端機指令，例如查詢日期、使用者名稱、目前目錄，以及列出資料夾內容。

---

## 二、我給 Agent 的問題

請你實際使用 terminal 工具完成以下任務，不要只用文字說明。

任務：
1. 顯示目前日期與時間
2. 顯示目前使用者名稱
3. 顯示目前所在目錄
4. 列出桌面資料夾中前 5 個檔案或資料夾

請回傳：
1. 你使用了什麼工具
2. 你執行了哪些指令
3. 終端機回傳的實際結果
4. 簡短說明這代表你有完成 tool calling

---

## 三、Agent 的執行過程

Agent 表示本次使用 terminal 工具執行任務。

任務 1：顯示目前日期與時間

💻 terminal: "date"

任務 2：顯示目前使用者名稱

💻 terminal: "whoami"

任務 3：顯示目前所在目錄

💻 terminal: "pwd"

任務 4：列出桌面資料夾中前 5 個檔案或資料夾

💻 terminal: "ls -lt ~/Desktop | head -n 5"


---

## 四、Agent 的回答

好的，身為你的人文導論課程助教，我這就來實際操作 Terminal 工具，為你完成這些任務！

1. 使用的工具

我會使用 terminal 這個工具來執行你交代的指令。

2. 執行的指令與終端機回傳結果

任務 1：顯示目前日期與時間

💻 terminal: "date"

終端機回傳結果：
Mon May  4 19:01:40 CST 2026

任務 2：顯示目前使用者名稱

💻 terminal: "whoami"
💻 terminal: "pwd"

終端機回傳結果：
berneting

任務 3：顯示目前所在目錄

終端機回傳結果：
/Users/berneting

任務 4：列出桌面資料夾中前 5 個檔案或資料夾

💻 terminal: "ls -lt ~/Desktop | head -n 5"

終端機回傳結果：
total 4061120
-rw-r--r--@   1 berneting  staff      19657 May  3 11:44 教育部文藝獎.docx
-rw-r--r--@   1 berneting  staff    3202954 May  1 20:29 截圖 2026-05-01 晚上8.29.54.png
-rw-r--r--@   1 berneting  staff     317412 May  1 11:23 截圖 2026-05-01 上午11.23.00.png
-rw-r--r--@   1 berneting  staff    1579542 Apr 30 10:50 截圖 2026-04-30 上午10.50.38.png

透過上面這幾次的操作，我實際使用了 terminal 這個工具，並且成功執行了你指定的指令，也將終端機的回傳結果呈現出來。這就代表我完成了「Tool Calling」的任務。
---

## 五、我的觀察

這次任務不是單純問答，因為 Agent 需要取得我電腦目前的時間、使用者名稱、所在目錄，以及桌面資料夾內容。這些資訊必須透過 terminal 工具實際執行指令才能取得。
因此，Agent 若有顯示它呼叫 terminal 工具，並回傳實際終端機結果，就符合 Tool Calling 的成功標準。
