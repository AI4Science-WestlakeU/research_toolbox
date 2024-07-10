# 有用科研工具集锦
[网页版](https://ai4s.lab.westlake.edu.cn/blogs/2024/04/10/%E6%9C%89%E7%94%A8%E7%A7%91%E7%A0%94%E5%B7%A5%E5%85%B7%E9%9B%86%E9%94%A6.html)

## 引言

"工欲善其事，必先利其器"当然说的很好，行军打仗，选择一件称手的兵器自然是上阵的前提。作为科研工作者，我们怎么做文献调研？怎么阅读和管理文献？怎么更加高效的设计和实施实验？如何快速完成论文写作中语言润色、画图、编辑公式等等都是费时费力的工作等等。作为计算机科学方向科研小白的我刚入门时，自己摸索文献调研、实验记录、论文写作等等走了不少弯路，很多时候一问老师同学或者上网找经验，原来有捷径啊？原来不需要一个个手动操作？由此便有了这一篇博客，记录和分享科研经历中的一些有意思的工具。

## 领域调研/文献管理

1. paper搜索/下载
    
    1. 开题的时候想快速调研一个领域？有了idea想快速找到相关文献？灵感枯竭想找点有意思的paper？别急，这里都有。
    
    |  | 工具/网站 | 特点 |
    | --- | --- | --- |
    | 搜索引擎 | Google/Edge | 信息丰富。一些相关博客、开源repo等也会列出 |
    |  | 插件:[Scihub addon](https://chromewebstore.google.com/detail/scihub-addon/hfcbmognahkfhdhfhfgiioafohojeolh?hl=zh-CN&utm_source=ext_sidebar), [Sangerboxnote](https://chromewebstore.google.com/detail/sangerboxnote/hblcedloibomgfngblmmmaoddadbdonj?hl=zh-CN&utm_source=ext_sidebar), [EasyScholar](https://www.easyscholar.cc/download) | 装上插件的浏览器直接如虎添翼，这几个插件显示论文期刊分区、IF、学科分类，帮我们方便快速定位当前文章质量 |
    | 学术网站 | [Google scholar](https://scholar.google.com/schhp?hl=zh-CN) | 查找文献的首选，论文质量比较好，还有一些社交订阅等功能，但是文章更新稍有延迟 |
    |  | [Semantic scholar](https://www.semanticscholar.org/me/research) | 支持语义搜索，文献更新较快 |
    |  | [Web of Science](https://www.webofscience.com/wos/) | 资源丰富，非免费 |
    |  | [中国知网](https://www.cnki.net/) | 除此之外的[万方](https://www.wanfangdata.com.cn/)、[维普](https://qikan.cqvip.com/)等对中文文献非常友好 |
    | 工具 | 关联文献：[Connected papers](https://www.connectedpapers.com/) & [Research rabbit](https://www.researchrabbitapp.com/home) & [litmaps](https://www.litmaps.com/about/us) | 利用这两个工具，给定一篇paper，迅速找到相关的paper，标记时间和引用，快速找到该领域的大牛和重要paper |
    |  | 领域调研：[paperdigest](https://www.paperdigest.org/review/) & [aminer](https://www.aminer.cn/) | 利用LLM，输入领域描述可以帮助写一个简单review,列出related paper.还可以提问（指定会议），比如快速消化[ICLR 2024的热点paper](https://www.paperdigest.org/topic/?topic=iclr&year=2024)。并且[aminer](https://www.aminer.cn/) 支持按期刊水平等进行检索，可以根据排名方便找到该领域的重要paper、大牛以及新星，侧重AI领域的paper |
    |  | 其他： [researchgate](https://www.researchgate.net/) | 学术圈的facebook |
    | 下载 | 期刊官网 | 直接检索，进入官网下载 |
    |  | [arxiv](https://arxiv.org/) | 一个收集物理学、数学、计算机科学、生物学与数理经济学的论文预印本的网站 |
    |  | [SciHub](https://www.sci-hub.ee/) | 懂的都懂 |
    |  | [annas-archive](https://annas-archive.org/) | 电子书pdf，资源丰富 |
    |  | [网站集锦](https://www.ablesci.com/daohang) | 各种网站入口集锦 |
2. 阅读/管理
    
    找到了相关的paper，如何快速阅读？如何更加高效的管理文献？问题接踵而来，下面则是应对之策。
    
    |  | LLM支持工具网站：[chatpdf](https://www.chatpdf.com/)& [txyz](https://app.txyz.ai/) &[chatgpt](https://chat.openai.com/c/a8d2b965-8208-4097-8029-528bf10a925a) & [claude](https://www.anthropic.com/news/claude-2) | LLM驱动的文献快速阅读工具，通过上传pdf或者url等，帮你快速总结文献核心要点。 |
    | --- | --- | --- |
    |  | 笔记：[Notion](https://www.notion.so/) & [飞书](https://www.feishu.cn/) | 两个工具排版非常方便，支持多人协作文档编辑，还可以方便导出各种文件格式如docx、pdf、markdown、latex等格式 |
    | 管理 | [Endnote](https://endnote.com/zh/) | 文献管理，方便和word结合起来管理引用，教程比较全面，缺点是付费 |
    |  | [zotero](https://www.zotero.org/) | 开源，但是对中文文献不是特别友好 |
    | 集成式工具 | [ivysci](https://www.ivysci.com/) | 集成搜索、下载、阅读、笔记、管理甚至写作等功能 |

## 实验

1. 有用脚本
    
    计算机相关专业的从业者，往往需要大量与GPU、conda、服务器、git等名词后面的东西打交道，本节列举一些实验中常用脚本，方便使用。
    
    1. git相关（更多请参考[Git and GitHub](https://oxgvbje0rda.feishu.cn/wiki/N3FrwehgDi1DHfkin8fcjopBnAd?from=from_copylink)）
        
        ```bash
        # 信息配置
        git config --global user.email "XXX@email.com"
        git config --global user.name "NAME"
        
        ```
        
        这个错误通常是因为你没有在本地设置SSH密钥，或者你的SSH密钥没有添加到GitHub的SSH密钥列表中。你可以按照以下步骤来解决这个问题：
        
        ```bash
        ls -al ~/.ssh #查看你是否已经有一个SSH密钥。id_rsa.pub或者id_ed25519.pub等文件出现表示已存在SSH密钥
        ssh-keygen -t ed25519 -C "your_email@example.com" #若没有，创建一个新的SSH密钥
        eval "$(ssh-agent -s)" #确保ssh-agent是在后台运行的
        ssh-add ~/.ssh/id_ed25519 # 将SSH私钥添加到ssh-agent
        cat ~/.ssh/id_ed25519.pub # 复制输出。接着，打开GitHub网站，点击右上角的头像然后选择"Settings"，在左侧选择"SSH and GPG keys"，点击"New SSH key"，在"Key"字段中粘贴你刚刚复制的公钥。
        
        ```
        
        [Git ignore](https://www.runoob.com/linux/linux-vim.html)
        1. 创建.gitignore文件
        
        ```bash
            touch .gitignore
        ```
        
        2. 给.gitignore文件添加条目
        
        ```bash
        
        vim .gitignore
        i#进入编辑模式
        #编辑
        #Esc退出编辑模式
        :wq#保存
        ```
        
    2. conda环境管理
        
        ```bash
        conda create -n NAME python=3.6.1 # 创建开发环境
        pip list --format=freeze >requirements.txt #pip 导出配置文件
        pis install -r requirement.txt
        conda env export --no-builds > environment.yml
        conda env create -f environment.yml
        
        ```
        
        ```bash
        source /opt/conda/bin/activate #可能需要激活conda
        conda activate ENV_NAME
        python XXX.py
         export CUDA_VISIBLE_DEVICES=1; python XXX.py #指定GPU运行
        
        ```
        
    3. 文件
        
        ```bash
        # rsync文件下载
        rsync -avz --progress -e ssh YOUR_NAME@0.0.0.0:/mnt/inaisfs/user-fs/YOUR_SOURCE_PATH/ YOUR_TARGET_PATH/ #可以仿照在实验室服务器终端运行这个下载
        #文件压缩
        tar -czvf example.tar.gz example.txt
        tar -xzvf example.tar.gz #解压到当前文件夹
        
        ```
        
    4. 终端连接管理
        1. [tmux](https://www.jianshu.com/p/71999b35ead7) （防止ssh连接断开，提交的任务被终止）
        
        ```bash
        tmux new -s $session_name #创建并指定session名字
        tmux a -t $session_name  #进入已存在的session
        tmux ls #列出session
        tmux kill-session -t $session_name #删除指定session
        
        ```
        
    5. 代码调试
        
        ```bash
        import pdb
        pdb.set_trace() ##断点调试
        
        #%% #增加“#%%”可以变成单元格方便调试
        
        ```
        
    6. 有用python绘图脚本（持续更新中）[github repo](https://github.com/Zhangtao167/plot_tools)
    7. 项目code框架示意[模版](https://github.com/AI4Science-WestlakeU/standard_repo)（方便code管理和开发）
    8. 其他
        
        ```bash
        watch -t nvidia-smi #查看GPU使用情况
        jupyter nbconvert --to python NOTEBOOK.ipynb  #将ipynb文件转换为py文件
        
        ```
        
2. IDE
    
    虽然传言最强大的程序员使用文本编辑器编程，做到无剑胜有剑，初出茅庐的小白还是拘泥于器，下面则是我最喜欢的两个IDE，足以胜任所有编程工作。
    
    | [vscode](https://code.visualstudio.com/) | git相关插件 |[gitdiff](https://marketplace.visualstudio.com/items?itemName=donjayamanne.githistory) ：git diff功能，对比编辑历史，可视化更加方便、明显，并且在编辑的时候自动标记更改方便跟踪实时code修改 |
    | --- | --- | --- |
    |  |  | [gitlens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)：显示每一行的编辑历史,提示未commit的修改等 |
    |  | code相关 | [copilot](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot)：LLM驱动的编程助手，教育学生认证后免费 |
    |  |  | [EasyCodeAI](https://marketplace.visualstudio.com/items?itemName=EasyCodeAI.chatgpt-gpt4-gpt3-vscode) copilot的替补，LLM辅助解释程序和处理bug |
    |  | 其他 | [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)（文件路径补全）& [Image preview](https://marketplace.visualstudio.com/items?itemName=kisstkondoros.vscode-gutter-preview)（图片预览）&[vscode-pdef](https://marketplace.visualstudio.com/items?itemName=tomoki1207.pdf) & [Docx/ODT Viewer](https://marketplace.visualstudio.com/items?itemName=ShahilKumar.docxreaderz) & [file-size](https://marketplace.visualstudio.com/items?itemName=zh9528.file-size) |
    | 文件工具 | [Final shell](https://www.hostbuf.com/) | ssh链接后，上传和下载文件比较方便稳定，也自带编辑器编写简单的文本。 |
3. 实验记录

| 工具 | 飞书 & Notion | 方便协作和展示 |
| --- | --- | --- |
| 机器学习学习强相关 | [tensorboard](https://pytorch.org/docs/stable/tensorboard.html) | ◦ TensorFlow的官方可视化工具，与TensorFlow紧密集成，免费且开源，支持多种数据可视化类型，如标量、图像、音频、计算图等。    ◦ 功能相对基础，主要针对Tensorflow架构 |
|  | [wandb](https://wandb.ai/site) | ◦ 云端服务，方便远程访问实验数据，支持大量的机器学习框架，强大的可视化和报告生成功能，实时监控实验状态，以及与团队成员共享实验结果的功能。    ◦ 需要联网，免费版存储空间和功能有限 |
|  | [mlflow](https://mlflow.org/) | ◦ 开源且支持多种机器学习框架，提供了实验跟踪、模型打包、模型服务部署等全套机器学习生命周期管理功能，可以部署在本地或云端，灵活性高。    ◦ 相比WandB和TensorBoard，社区支持和用户基础较小，配置和使用相对复杂。 |
|  | [Comet.ml](https://www.comet.com/site/) | ◦ 提供实验跟踪、参数优化等功能，强大的可视化工具和云端存储，支持代码版本控制和实验比较。    ◦ 免费版本功能有限，完整功能需要付费,需要联网。 |
|  | [ClearML](https://clear.ml/) | ◦ 提供了一个端到端的MLOps平台，支持实验跟踪、数据管理、模型部署等。强大的自动化机器学习流程，支持云端和本地部署。    ◦ 对于初学者来说，功能丰富可能导致上手难度较高，企业级功能需要付费。 |

## 论文写作

论文的写作问题令很多人头疼不已，无论是排版、文法、画图等等，都是一个个棘手的挑战。可能是繁琐的低脑力重复工作，可能是文法上当局者迷，也可能是画图是感叹艺术细胞缺失，下面是一些工具帮助解决这些问题。

| 文本 | [overleaf](https://www.overleaf.com/) | 在线latex开发工具，支持多人协作 |
| --- | --- | --- |
|  | [word](https://www.microsoft.com/en-us/microsoft-365/free-office-online-for-the-web) | 质朴万能工具 |
| 公式 | [在线latex公式编辑](https://www.latexlive.com/) | 在线公式编辑，方便预览和导出，notion也可以方便导出 |
|  | [在线表格转换工具](https://tableconvert.com/zh-cn/excel-to-markdown) | 在线表格转化 |
|  | [Mathpix snip](https://mathpix.com/) | 扣其他论文的公式，也可以使用GPT4 |
| 表格 | [在线生成表格](https://www.tablesgenerator.com/latex_tables) | 在线表格生成编辑，方便导出latex、markdown、html等格式 |
| 图 | 示意图：PPT & Visio & origin | 方便快捷，支持多种模版，方便展示 |
|  | 数据图：Python & Matlab | 方便自己调试，自由度高 |
|  | PPT素材：[ML相关](https://github.com/dair-ai/ml-visuals?tab=readme-ov-file) | 套用一些PPT模版或者素材，减少重复性劳动 |
| 其他 | 语法：[grammarly](https://app.grammarly.com/) | 支持边写边结错，可设置全局使用 |
|  | 润色：[ChatGPT](https://chat.openai.com/) | 注意辨别用词，LLM此处倾向使用高级词汇 |

## 其他

### 一些其他工具科研生活中也必不可少，如文件格式转换、文件查找等，持续更新中......

| 文件 | [Convertio](https://convertio.co/zh/) | 在线免费网站，支持多种文件格式相互转换 |
| --- | --- | --- |
|  | [Everything](https://www.voidtools.com/zh-cn/downloads/) | 本地文件查找 |
| 笔记 | xmind | 热门思维导图软件，笔记和展示都非常方便美观 |
| 其他 | [Autothink插件](https://app.autothink.io/) | outlook插件，自动根据来信回复邮件 |
|  | [blog](https://blog.csdn.net/weixin_51100018/article/details/130438900) | 完成基本信息替换即可搭建个人学术主页 |

### **其他补充（in updating）**

1. Anonymize code repo with anonymous github
    1. Create a private repo: PROJECT_NAME
    2. Add your code to this repo (be careful to delete the personal information)
    3. Use https://anonymous.4open.science/ to get anonymous repo
    4. Share the anonymous repo link