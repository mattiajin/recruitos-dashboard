# RecruitOS Dashboard

招聘供应商与数据分析系统 · UI 原型（v1.0 · Vivid Sky）

静态单页原型，可直接部署到 GitHub Pages 或任意静态托管。

## 在线预览

部署完成后访问：

```
https://<your-username>.github.io/<repo-name>/
```

## 本地预览

```bash
# 方式 1：直接打开
open index.html

# 方式 2：本地静态服务（推荐）
python3 -m http.server 8080
# 浏览器打开 http://localhost:8080
```

## 仓库结构

```
├── index.html          # 主原型（New Design 默认）
├── README.md           # 本文件
├── 设计师交接.md       # 接手必读
├── 设计.md             # UI 规范
├── 动画.md             # 动效规范
├── 文案对照.md         # 中英文文案
└── legacy/             # 早期 phase1 稿（仅供参考）
```

## 原型 Tab

| Tab | 说明 |
|-----|------|
| Original | 旧版对照 |
| **New Design** | 正式稿（默认） |
| Specs | 设计规范（英文） |
| Themes | 备选配色预览 |

右上角 **中文 / EN** 切换界面语言。

## 部署 · GitHub Pages

### 方式 A：GitHub Actions（推荐，已配置）

1. 将本仓库 push 到 GitHub
2. 进入 **Settings → Pages**
3. **Source** 选择 **GitHub Actions**
4. push 到 `main` 分支后自动部署

### 方式 B：静态分支

1. **Settings → Pages**
2. **Source**：Deploy from branch
3. Branch：`main` · Folder：`/ (root)`
4. Save

### 其他平台

| 平台 | 说明 |
|------|------|
| Vercel / Netlify | 导入仓库，Publish directory 填 `.` 或 root |
| 内网静态服务器 | 上传整个仓库根目录 |

## 依赖

- 字体：Google Fonts · DM Sans（CDN）
- 图标：Phosphor Icons（CDN）

需可访问外网 CDN；离线环境需改为本地资源。

## 文档

| 文件 | 内容 |
|------|------|
| [设计师交接.md](./设计师交接.md) | 交付说明、限制、待办 |
| [设计.md](./设计.md) | 完整 UI 规范 |
| [动画.md](./动画.md) | 动效规范 |
| [文案对照.md](./文案对照.md) | 文案中英对照 |
