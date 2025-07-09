
MY INSTALLATION TOUR GUIDE


==========================================
* 先從外接印碟, 安裝 Install\tools\Backup
  * use "load from E to D" for backup. 


==========================================
Whenever reinstall the whole MS windows, please install by default the following: 

* Make Windows updated
  * KMS (renew, 有版權的不用) 
    * 每半年Office 選: Office LTSC 2021

* Install MS Office. 
  * KMS (renew) 
    * 每半年Office 選: Office LTSC 2021

* Install Anti-virus Norton or Avira (小紅傘).
  * 其他功能 -> 組態 -> 網際網路防護 -> mail protection -> 掃描 -> 偵測所發現病毒時動作 -> 自動
    避免讀信時, 反覆詢問

(X) * Install visual dotnet for writing programs:

(X) * Install Acrobat: (Use PDFXViewer instead)
  * \cdrom\Acrobat6.0
  * License: 1016-1206-1067-2427-4942-9333

* Install Chrome
* Install everything
  * To avoid C:\Virtual Disk, add the following to C:, C:\GoogleDrive1;C:\GoogleDrive-g2;C:\Program Files;C:\Program Files (x86);C:\ProgramData;C:\Users\icwu;C:\Windows

==========================================
Above could be done by system manager. 

* 中文輸入
  * "語言喜好設定" -> "中文(台灣)" --> "選項" --> "微軟注音" --> "選項" --> "開啟進階設定" 
    (old: set to 新注音 and 羅馬拼音.)
  * "語言設定" -> "中文(繁體, 台灣)" --> 按圖 "abc v" --> "選項" --> "微軟注音" --> "選項" --> 
    * "按鍵指派" --> 選擇輸入法
  * "學習" --> "開啟使用者造句" (似乎不用改輸入法了)
    * 直接搜尋 "學習" 或 "開啟使用者造句"?
  * Install 詞彙 by importing (匯入) D:\Documents and Settings\My Documents\phrases\dict.txt. 
  (ignore Hanin any more)

* Install GoogleDrive
  * Download GoogleDrive, install it, 
  * icwu307@gmail.com --> C:\GoogleDrive1
    * Backup and Sync From Google
  * icwu307@g2.nctu.edu.tw --> C:\GoogleDrive-g2
    * Backup and Sync From Google (simply use "Add New Account" from the previous one)
  * icwu307@nctu.edu.tw --> G:\ 
    * Use "Google Drive File Stream"
  * 再來 "新增帳戶" (D:\GoogleDrive-g2)

* Maintain some files in backup disk (copied back from the disk)
  * books
  * old_cvs
  * distlab (use backup to get the latest)
  * distlab-photos
  * video-course

* update VS Code for icwu307.github.io (https://code.visualstudio.com)
  * files are in D:\github\icwu307.github.io
  * Go go to "source control"
    * update: click on the icon "source control", type a message "update message" and then click on "commit". 
    * Sync: click on "Sync Changes" (note: must kill the window of "message" in case of no resposnes. 
    * Need to select "commit" again (in "..."). 
  * need to download Git for windows? 
  * Initially for a new NB, we need to do the following: 
    * open view TERMINAL, then click on TERMINAL
  * run the following:
    git config user.name
    >>
    PS D:\github\icwu307.github.io> git config --global user.name "icwu"
    PS D:\github\icwu307.github.io> git config --global user.email "icwu@cs.nycu.edu.tw"
    PS D:\github\icwu307.github.io> git config user.name

==========================================
Now, start loading "Documents and Settings\". 
Note: some may use the files under "\cdrom" from some BACKUP_HD. 

* If use virtual disk, run 'subst D: "C:\Virtual Disk"'
  * set everything's indexing C: to "C:\GoogleDrive;C:\Program Files;C:\Program Files (x86);C:\ProgramData;C:\Windows;C:\Users"
  * 重開機會關掉, 參考 GPT 的建議用 task scheduler. (很好用!)

* Change password.

* Change some settings: 
  * (不要管,反正都在 C:\Users\icwu\) Note: all in "D:\Documents and Settings\" are moved to "C:\Users\icwu"
    * "D:\Documents and Settings\My Documents" --> "C:\Users\icwu\Documents"
  * backup "C:\Users\icwu", instead. 
  * Change "C:\Users\icwu\Pictures\我的相簿" to "C:\GoogleDrive-g2\我的相簿"
  * In Chrome settings: 
    * "My favorites": Set to "D:\Documents and Settings\My Documents\Favorites\bookmarks_13_8_30.htm" 
    * "繼續瀏覽上次開啟的網頁", (continue where you left out)
    * "檔案下載儲存位置" (C:\Users\icwu\Downloads)
    * 字型大小 (to large)
  * 變更 Chrome 的磁碟快取目錄位置 http://blog.joaoko.net/archives/2957

* Install\tools\
  * everything
  * Refresh Explorer: "Refresh Explorer.vbs"
  * Backup 
    * Set up backup link on desktop D:\Documents and Settings\reinstall\backup
  * procExplorer
  * SSH
  * svn
    * in D:\Documents and Settings\reinstall\tools\svn\TortoiseSVN-1.8.1.24570-x64-svn-1.8.1
  * 7zip
  * videolan 
  * iphone's photo 
  * switch "相機" 的 "格式" 從 "高效率" 到 "最相容"
      不然都是用 *.heic, 需要 heic-trans 轉換
    * switch "照片" 的 "格式" 從 "自動" 到 "保留原始檔案". 
  * 縮圖問題: 安裝 k-lite. 
  * Run Codec Tweak Tool, for "Miscellaneous", click on "Thumbnails" and then "select all" and click "Apply&close". 
  * notepad++ 
    * 檢視 (View) --> 自動斷行 (Word Wrap)
  * set 邊緣線設定


* 資料夾選項: (檔案總管 File Explorer)
  * "檢視" -->　展開到目前資料夾. (expand to open folder)
  * "view" --> 隱藏附檔名. (show hidden files, ...) 

* 插電時候, 不睡眠

* Install ca.nctu.edu.tw

* iphone backup 備份:
  * use iTunes for backup
    * iPhone 備份到電腦 Windows
    用連接線連接iPhone和電腦
    選擇電腦的iTunes App，並點擊 iTunes 視窗左上角的 iPhone 按鈕 (很小的手機 icon)
    點擊「摘要」
    在「備份」下方，按下「立即備份」
    若需要加密備份資料，請選擇「替本機備份加密」
  * 電腦備份到 iphone (還沒有試過)
  * Files are stored in C:\Users\icwu\Apple\MobileSync\Backup
    * 為了省空間, 存到備份硬碟的 iphone-backup\

==========================================
Take a break and then do the following, if necessary.

* Outlook
  * Install Outlook.  (最好裝2019)
    * 新版 Outlook 啟動時會詢問伺服器類型，請選擇「POP3」。如有需要，可刪除並重新建立「個人資料夾」。
    * 使用「檔案」>「帳戶設定」來設定多個郵件帳號。
      * 請選擇「手動設定...」才能設定 POP3。
      * 建議使用「icwu@cs」等帳號，以便套用規則。
    * 若需更改「個人資料夾」：
      * 先新增「個人資料夾」。
      * 進入「檔案」>「帳戶設定」>「資料檔」，將預設資料檔改為「個人資料夾」。
      * 有時安裝時可直接選擇，若無則可先「變更資料夾」或刪除後重新新增。
      * 到「傳送/接收」>「傳送/接收群組」>「定義傳送/接收群組」，設定不要隨時收信，可排程自動收發的間隔時間。
      * 新版 Outlook 可用「修復」功能檢查或修改。
    * 垃圾郵件選項請設為「高」。
    * 以下為舊方法，僅供參考：
      * 若需更改「個人資料夾」位置，請先將郵件接收資料夾設為其他位置（工具 > 郵件帳號 > 設定接收資料夾）。
      * 更改後，新的備忘錄、行事曆、聯絡人會顯示於新位置。
      * 匯入帳號：settings\*.iaf
      * 匯入聯絡人：settings\mine.wab
      * 匯入規則：settings\outlook-email-rules.rwz（很重要）
      * 設定簽名檔。
    * 設定規則（大多數帳號都需檢查）。完成下列工作後，請至「規則」>「管理規則」>「套用」。
    * 設定簽名檔。
    * common-email-list.txt：設定所有常用自動完成功能（也可參考 docs.google.com/實驗室文件、群組名單）。

==========================================
Add the following when have more times. 

* zotero https://www.zotero.org/groups/5129226/rlg-papers?token=44ilofln73sm3d2y7i34pcou8jihzvm785p6f0ni

* Install Skype
  * SkypeSetup.exe

* Install links to 119, shared and printers
  * setup D:\shared to \\140.113.167.109\shared
  * setup \\140.113.167.109 printers. 
  * 去設定裝置和印表機
  直接按新增印表機
  應該就會出現了
  要注意看印表機的 room number (e.g., 511 or 517)

* Install HTC-sync. 

* Install PDFXViewer (free version is very good)
  D:\Documents and Settings\reinstall\PDFXViewer

* Install Firefox. 

* VPN:Pulse Secure 
  * 下載 WireGuard
  * 下載通道: C:\Users\icwu\Documents\VPN-Channels-通道\ CGILab-1.conf ~ CGILab-4.conf

* 視窗背景顏色: "設定" --> "個人化" "背景主題" "彩色"
  "協助工具" -> "字體大小" (120%?)
  -> "視覺效果" -> "動畫效果", "透明效果"

* Connect to CGI NAS-511
  要先連上 VPN http://vpn.cgilab.nctu.edu.tw/
  下載 config (in OpenVPN\config) 和對應的 client
  * 至於 \\aigames.nctu.edu.tw\ (我的網頁) 要去手動打開
  老師按 Win+R
  optionalfeatures
  Enter
  把 SMB 1.0.Client 打勾
  中文是 “SMB 1.0 客戶端

* Clean Gmail (Google drive)
  * "after:2015/12/31 before:2017/1/1"

* Teamviewer

* Install itunes, MobileSync
* Install GoGui, Goban, Drago
* Install Line, 
* Install Nodepad++, SSH, putty (as a backup for SSH)
* Install WinRAR, 7-zip

* MD Editor (see .\vscode-remote.html, in the same directory)
  * Download/Install Visual Studio Code (VS Code)
    * Extensions (one of left most icons, CTL-X)
  * search "Remote Development", then install it. 
  * In installer, check all options listed (in vscode-remote.html)
  * In CMD, run code --install-extension ms-vscode-remote.vscode-remote-extensionpack
  * Copy the folder \\aigames.nctu.edu.tw\icwu\.ssh into %USERPROFILE% (就是 C:\UsersFPD\icwu)


* Windows Command "optionalfeatures", "SMB 1.0/CIFS 檔案共用支援", "SMB 1.0/CIFS 用戶端".

* If toolbar does not work, 
  * CTRL-SHITF-ESC to invoke taskmaanager then type "taskkill /f /im explorer.exe"
  * explorer

==========================================
Add optionally some of the following (some are out of date): 

* Install NkView5 for Nikon's camera:  (X)
  * \reinstall\NkView5

* Install ghostview for reading some Postscript (PS) files.   (X)
  * \reinstall\ghostview\setup.exe

* Install Java JDK (X)
  * download the latest one

* Move 稅務系統！
  * IRX606.EXE???

* Install google_desktop

* Install goldwave for editing audio and music. 
  * lamewin32.exe (first)
  * gwave508.exe
    User ID: F3N6N8ATW
    License: F23EFCDK2

* Install Ghost
  * Then, backup your OS by using Ghost.  


* Install Nero6c and Nero6cht

* Install DWG (for 萊茵土地測量)
  * D:\Documents and Settings\reinstall\DWG
* Install python
  * 

http://www.tvbnow.com/viewthread.php?tid=267758
http://tw.search.yahoo.com/search?ei=UTF-8&p=%E9%99%B3%E5%86%A0%E5%B8%8C+%E8%A3%B8%E7%85%A7+download&pstart=1&fr=yfp&b=11


投資理財: (中國信託)
* 按 "基金" --> "標的代碼" 內之 高盛/PICO --> 利率是: 0.075(配息紀錄)*12(月)/9.52(參考申購淨值) --> 申購 (外幣申購)
























