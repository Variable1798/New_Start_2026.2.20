# 服务器常用指令
1. 新建（文件夹名）文件夹  
mkdir （文件夹名）
注：（确保父目录存在）如果你想一次性创建多层文件夹（例如 Project/KATO），但 Project 还没创建，可以使 用 -p 参数：  
mkdir -p Project/KATO  
2. 文件夹重命名  
rm -r "Untitled Folder"  
注意：文件夹要是有多个单词，一定要用双引号将全称括起来  
3. 移动文件至另一个文件夹  
1）将文件夹中所有文件都移动到新文件夹中  
mv * （文件夹名）/  
遵循规则：mv /路径/到/源文件夹/*.py /路径/到/目标文件夹/  
2）将文件夹中部分文件移动到新文件夹中 
mv /home/user/project/script.py /home/user/project/KATO/  
遵循规则：mv /路径/到/源文件夹/（文件名）.py /路径/到/目标文件夹/  
4. 切换服务器Terminal运行路径  
1）进入指定文件夹：  
cd KATO  
2）返回上一级目录：  
cd ..  
3）直接回到当前用户根目录：  
cd ~  
或者直接输入 cd 也可以  
4）进入绝对路径（从系统根目录开始）：  
cd /home/user/Documents/KATO