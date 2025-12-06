# 江男の颈椎守护者

一个基于 MediaPipe 的网页端颈椎姿态监测工具，旨在帮助久坐党保持健康的坐姿。

本项目核心代码由 **Gemini 3 Pro** 生成。

## 在线使用

无需安装，直接访问 GitHub Pages 即可使用：

👉 **[点击开始守护颈椎](https://xingye1673.github.io/NeckGuard/)**

*(注意：首次打开需要授予摄像头权限)*

## 项目地址

[https://github.com/xingye1673/NeckGuard](https://github.com/xingye1673/NeckGuard)

## 功能特点

- **实时姿态监测**：通过摄像头实时捕捉头部和肩部位置。
- **不良姿态预警**：当检测到低头、歪头或距离屏幕过近时，发出提醒。
- **久坐提醒**：内置计时器，提醒定时休息。
- **隐私保护**：所有计算完全在本地浏览器进行，视频流不上传服务器。

## 部署指南 (GitHub Pages)

本项目是一个纯静态网页应用，非常适合使用 GitHub Pages 免费部署。

1.  **Fork 或上传代码**：将本项目代码上传到你的 GitHub 仓库 (例如 `NeckGuard`)。
2.  **开启 Pages 服务**：
    - 进入仓库页面，点击 **Settings** (设置)。
    - 在左侧菜单找到 **Pages**。
    - 在 **Build and deployment** 下的 **Source** 选择 `Deploy from a branch`。
    - 在 **Branch** 选项中选择 `main` (或 `master`) 分支，文件夹选择 `/ (root)`。
    - 点击 **Save**。
3.  **获取链接**：等待几分钟后，刷新页面，你将看到生成的网站链接 (通常是 `https://你的用户名.github.io/仓库名/NeckGuard/`)。

## 本地调试

如果你想在本地运行或修改代码：

1.  **确保已安装 Python**。
2.  **在项目根目录下打开终端**。
3.  **运行以下命令启动服务**：

   ```bash
   python -m http.server 8000
   ```

4.  **打开浏览器访问**：[http://localhost:8000/NeckGuard/](http://localhost:8000/NeckGuard/)

### 注意事项

- **摄像头权限**：浏览器通常只允许在 HTTPS 环境或 `localhost` 下调用摄像头。如果你在局域网内部署 (如 `192.168.x.x`)，需要配置 SSL 证书，否则摄像头无法启动。使用 GitHub Pages 部署会自动获得 HTTPS 支持，推荐使用此方式。

---
*Made for my wife.*
