# 刘瑞洋的个人网站

单文件静态个人主页，零依赖，直接用 GitHub Pages 托管。

- 线上地址：https://liury991-cpu.github.io
- 技术：纯 HTML / CSS / JS（`index.html` 单文件）

## 模块结构

1. **Hero 首屏** — 自我介绍 + 照片位 + 视频位
2. **Works 作品集** — Web Coding 项目（记忆罐 / 旅行 AI 助手 / 更多 GitHub 项目）
3. **Journey 经历** — 实习 + 教育时间线
4. **Life 生活切片** — 摄影 / 音乐 / 调酒 / 运动 + My AI Workflow
5. **Contact** — 邮箱 / 微信 / GitHub

## 素材替换指引

所有待替换的位置都在 `index.html` 中以 `TODO(...)` 注释标出：

| 内容 | 操作 |
|---|---|
| 个人照片 | 照片放入 `assets/img/`（如 `me.jpg`），在 Hero 区搜索 `TODO(照片)`，删除占位 SVG 和 "PHOTO HERE" 标签，启用 `<img>` |
| 自我介绍视频 | 视频放入 `assets/video/`（如 `intro.mp4`），搜索 `TODO(视频)`，替换 `.video-slot` 内的占位内容为 `<video>` 标签 |
| 项目截图 | 截图放入 `assets/img/`，在 Works 区搜索 `TODO(截图)`，替换对应卡片 |
| 摄影作品 | 照片放入 `assets/img/`，在 Life 区搜索 `TODO(照片)`，替换三个照片占位槽 |
| 歌单 | 搜索 `TODO(歌单)`，增删歌曲（当前：keshi、方大同） |
| 酒单 | 搜索 `TODO(酒单)`，把 3 款占位鸡尾酒换成常调/爱喝的酒 |
| 经历数据 | Journey 区的数字成果为简历初稿数据，核实后直接修改对应文本 |

## 本地预览

直接双击打开 `index.html`，或：

```bash
python3 -m http.server 8000
# 浏览器访问 http://localhost:8000
```

## 部署（GitHub Pages）

本仓库名为 `liury991-cpu.github.io` 时，GitHub Pages 自动开启，push 到 main 分支即生效。
