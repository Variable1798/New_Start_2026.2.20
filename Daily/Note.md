## 笔记格式
New_Start_2026.2.20/  
├─ README.md  
├─ .gitignore  
├─ Daily/                  # 日记/流水账（按日期） 
│  ├─ 2026-02-20.md  
│  ├─ 2026-02-21.md  
│  └─ assets/              # Daily 专用小图（可选） 
│     └─ 2026-02-20_ssh.png  
├─ Projects/               # 项目型笔记（按项目）  
│  ├─ GPR_DL_Inversion/  
│  │  ├─ notes.md  
│  │  └─ assets/  
│  └─ CE_LPR_Processing/  
│     ├─ notes.md  
│     └─ assets/  
├─ Topics/                 # 主题型知识卡片（按主题）  
│  ├─ Git.md  
│  ├─ SSH.md  
│  ├─ FDTD.md   
│  └─ KirchhoffMigration.md  
└─ Inbox/                  # 临时草稿/待整理  
   └─ quick_notes.md  
## 图片命名  
![](assets/2026-02-20_git_proxy_01.png)  
## git上传  
<mark> 原理 </mark>  
加内容  
告诉git你干了啥  
上传  
<mark> 示例 </mark>  
git status  
git add .  
git commit -m "2026-02-21 daily notes"  
git push  
<mark> 或 </mark>  
git add .gitignore  
git commit -m "update gitignore"  
git push  
<mark> 删除内容 </mark>   
git rm Daily/image.png    
git rm Daily/image-1.png  
git commit -m "remove unnecessary images"  
git push  
<mark> 替换名字 </mark>   
git mv Daily\image.png Daily\assets\2026-02-20_git_01.png  
git mv Daily\image-1.png Daily\assets\2026-02-20_git_02.png  