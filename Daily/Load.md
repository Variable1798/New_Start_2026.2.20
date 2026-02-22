# 如何向服务器上传数据集
## 前情提要：服务器端已经储存了你电脑的公钥，要是没有就输密码，一样的，免密登录教程看SSH.md
管理员身份启动Powershell，你的数据存在哪个盘就取哪个盘，这里以G盘举例，执行  
G:  
cd 你的分支文件夹（没有则忽略）  
tar -czvf （你的数据所在文件夹名）.tar.gz   
然后执行：  
sftp -P 40019 -i C:\Users\Quasar\.ssh\id_ed25519 jovyan@（你的服务器ip）  
pwd  
put （你的数据所在文件夹名）.tar.gz  
结果如图所示就算成功：  
![](assets\2026-02-22_git_01.png)   
执行：  
bye，退出sftp  
连接服务器，执行：  
ssh -p 40019 -i ~/.ssh/id_ed25519 jovyan@（你的服务器ip）  
结果如图所示就算成功：  
![](assets\2026-02-22_git_02.png)  
成功连接服务器！  
## 如果你要解压到指定目录（目录名以project为例）
执行：   
mkdir -p ~/projects  
tar -xzvf （你的数据所在文件夹名）.tar.gz -C ~/projects   
cd ~/projects/（你的数据所在文件夹名）  
## 或者直接解压
cd ~    
ls -lh transunet.tar.gz  （确认文件是否已经上传至服务器）  
结果如图所示就算成功：  
![](assets\2026-02-22_git_03.png)  
再执行解压  
tar -xzvf gdlc1.tar.gz   
最后断开服务器连接  
exit 