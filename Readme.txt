什麼？Linux 終端也可以用來看女神照片？[樹梅派/VPS 使用終端機(文字模式)顯示照片 ~ lsix] (LINUX Console show Image with lsix)


資料來源: https://mp.weixin.qq.com/s/qAoDLzq1ZwliNs-BbXGFSg

01.安裝相依套件 imagemagick

sudo apt-get install imagemagick

02.下載lsix + 解壓縮 + 拷貝到指定目錄 + 賦予執行權限 [LINUX 安裝 SHELL檔 /無相依二進制執行檔 SOP]

wget https://github.com/hackerb9/lsix/archive/master.zip
unzip lsix-master.zip
sudo cp lsix-master/lsix /usr/local/bin/
sudo chmod +x /usr/local/bin/lsix

03.啟動工作環境[xterm]
xterm -ti vt340

04.實測使用指令

[顯示當前目錄下所有圖片]
lsix
[顯示當前目錄下所有jpg圖片]
lsix *.jpg