開始吧!
===
1. 首先希望大家都可以擁有自己的[GitHub](https://github.com/)和[Docker Hub](https://hub.docker.com/)，這樣以後共同開發會方便很多<br>
2. 下方資料部分參考下方所有連結
---
目錄
* 網路攻擊
    * [網路滲透作業系統(Kali Linux)](#三網路滲透作業系統kali-linux)
    * [搜尋引擎滲透(Google Hacking)](#四搜尋引擎滲透google-hacking)
* 程式開發
    * [基礎程式語言(python)](#一基礎程式語言python)
    * [基礎虛擬化技術(Docker)](#二基礎虛擬化技術docker)
---
## 一、基礎程式語言(python)
* [Python官方](https://www.python.org/)<br>
    下載python
* [菜鳥教程](http://www.runoob.com/python/python-tutorial.html)<br>
    不必看完，但要用的時候找的到
* [程式語言教學誌](http://kaiching.org/pydoing/python.html)<br>
    不必看完，但要用的時候找的到
* [Python 基础入門教程](https://alleniverson.gitbooks.io/python2-course/content/)<br>
    不必看完，但要用的時候找的到
### 小問題
* pip安裝
  - 下載[get-pip.py](https://bootstrap.pypa.io/get-pip.py)
  - 開啟cmd執行 `python get-pip.py`
  - 最後加入 `C:\Python27\Scripts` 到環境變數中
### 測驗
    請練習菜鳥教程-100例中第1、3、8、24、26、32、34、61、71、83、85、88、97和100題。
---
## 二、基礎虛擬化技術(Docker)
* [Docker —— 從入門到實踐](https://philipzheng.gitbooks.io/docker_practice/content/)<br>
    請看完 Docker簡介、基本概念、安裝、映像檔、容器、倉庫和Dockerfile，其他不必看完，但要用的時候找的到
* [Docker Hub](https://hub.docker.com/)<br>
    目前由Docker官方維護的公共倉庫 Docker Hub，且Docker Hub 中可直接下載他人或官方的映像檔來使用
### 小問題
* 關於Docker下的alpine
  - alpine原本並沒有bash，所以要遠端登入時可使用sh來遠端登入
### 測驗
    請使用Docker建立一個FTP伺服器在Ubuntu中
---
## 三、網路滲透作業系統(Kali Linux)
* [Kali Linux 官方](https://www.kali.org/)<br>
    下載Kali
* [Docker版 Kali Linux](https://hub.docker.com/r/kalilinux/kali-linux-docker/)<br>
    如果常用Docker的人可以試試，但工具部分沒有其他版本那麼齊全
### 小問題
* 如何開啟Kail後自動登入桌面
  - 輸入 `vi /etc/gdm3/daemon.conf`
  - 將 `#AutomaticLoginEnable = True` 和 `#AutomaticLogin = root` 的 # 刪除
* 如何設定SSH遠端登入
  - 輸入 `vi /etc/rc.local`
  - 增加 `/etc/init.d/ssh start`
  - 輸入 `vi /etc/ssh/sshd_config`
  - 修改 `PermitRootLogin without-password` 為 `PermitRootLogin yes`
### 測驗
    暫無
---
## 四、搜尋引擎滲透(Google Hacking)
* [宅學習 - Social Learning Space](https://sls.weco.net/node/12922)<br>
    裏頭有非常多常用的手法可以應用在滲透上
* [GoogleHacking基礎](http://www.vixual.net/blog/archives/152)<br>
    裏頭有非常多常用的手法可以應用在滲透上
* [exploit-db實戰範例](https://www.exploit-db.com/google-hacking-database/)<br>
    裏頭有非常多常用的手法可以應用在滲透上
* [信息收集篇————Google Hacking](https://blog.csdn.net/Fly_hps/article/details/79404270)<br>
    裏頭有非常多常用的手法可以應用在滲透上
* 基礎指令介紹
  - site: (搜尋特定網址)
  - inurl: (搜尋特定連結)
  - intext: (搜尋網頁內文字)
  - intitle: (搜尋網頁標題)
  - filetype  |  ext  : (搜尋特定檔案格式)
  - link: (搜尋互相連結的網頁)
  - cache: (顯示網頁在Google中的暫存資料)
  - info: (列出某網站在Google上存有哪些資訊)
* 常用指令集
  - inurl:admin
  - inurl:phpinfo.php
  - intitle:index of 學生證
---
### 開發中...
