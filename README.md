\# 深圳游戏企业可视化报告



> 基于 JavaScript + ECharts 的深圳市游戏企业数据可视化报告



\## 📌 项目简介



本项目是一个专注于\*\*深圳市游戏企业\*\*的数据可视化报告页面。通过 ECharts 图表库，将深圳市游戏企业的分布、规模、类型等数据以直观的图表形式呈现，帮助读者快速了解深圳游戏产业的整体格局。



\## 🚀 在线预览



（如已部署 GitHub Pages，请将链接粘贴至此）



\## 📂 项目结构

├── 项目代码.html # 主页面（包含所有图表）

├── style.css # 页面样式

├── data.json # 数据文件

├── 深圳市.geojson # 深圳地图 GeoJSON 数据

└── README.md # 项目说明



text



\## 💻 如何下载到本地使用



\### 方式一：直接下载 ZIP（最简单）



1\. 点击页面右上角的绿色 `Code` 按钮

2\. 选择 `Download ZIP`

3\. 解压到本地文件夹

4\. 用浏览器打开 `项目代码.html` 即可运行（注意阅读下方浏览器配置说明）



\### 方式二：使用 Git 克隆



```bash

git clone https://github.com/baiyu-JW/baiyu-echarts.git

cd baiyu-echarts

⚙️ 浏览器配置说明（重要！）

⚠️ 本页面使用 fetch 异步加载本地 data.json 和 深圳市.geojson 文件。由于浏览器的跨域安全策略（CORS），直接用浏览器打开 项目代码.html 会导致数据加载失败（控制台会报 CORS 错误）。



🥇 方案一：VS Code Live Server（最推荐）

在 VS Code 中打开本项目文件夹



安装插件 Live Server（扩展 ID: ritwickdey.LiveServer）



右键点击 项目代码.html → 选择 Open with Live Server



页面将在 http://127.0.0.1:5500 自动打开，数据正常加载 ✅



优点：一键启动，自动刷新，完全不需要配置。



🥈 方案二：Python 简易 HTTP 服务器

在项目目录下打开终端，执行：



bash

\# Python 3

python -m http.server 8080

然后在浏览器访问 http://localhost:8080/项目代码.html



优点：电脑自带 Python 的话不需要额外安装任何东西。



🥉 方案三：Node.js http-server

bash

\# 全局安装 http-server（只需一次）

npm install -g http-server



\# 在项目目录启动

http-server

⚠️ 方案四：修改浏览器启动参数（不推荐，仅作备选）

如果你实在不想搭建本地服务器，可以通过修改浏览器启动参数来绕过跨域限制。但请注意：这会降低浏览器的安全性，建议仅在本地开发时临时使用，用完后恢复。



Chrome 浏览器

完全关闭所有 Chrome 窗口（检查任务管理器确保没有 Chrome 进程在后台运行）



按 Win + R，输入以下命令（注意替换路径中的用户名）：



bash

"C:\\Program Files\\Google\\Chrome\\Application\\chrome.exe" --allow-file-access-from-files

在打开的 Chrome 中，用 Ctrl + O 打开 项目代码.html 文件，数据即可正常加载



⚠️ 每次启动 Chrome 都需要加这个参数，否则会失效。



Edge 浏览器

bash

"C:\\Program Files (x86)\\Microsoft\\Edge\\Application\\msedge.exe" --allow-file-access-from-files

