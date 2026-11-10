# 我的工作台（GitHub Pages 部署包）

一个导航首页 + 三个单文件静态工作台，全部零后端，数据存在浏览器本地。

## 文件说明

| 文件 | 是什么 |
|---|---|
| `index.html` | 导航首页（打开仓库网址看到的第一个页面） |
| `learning-dashboard.html` | 任务工作台（学习看板） |
| `screenwrite.html` | 编剧工作台本体（**需你自行导出放入**，见下） |
| `api-screenwrite-tool.html` | 编剧备份调取工具 |

## 部署步骤（一次搞定）

1. 在 GitHub 新建一个**空仓库**（例如叫 `my-workbench`）。
2. 把本文件夹里的 **所有文件** 上传 / 推送到该仓库（可直接在网页端拖拽上传）。
3. 进入仓库 **Settings → Pages**：
   - Source 选 **Deploy from a branch**
   - Branch 选 **main** ，目录选 **/ (root)**
   - 点 Save。
4. 等一两分钟，访问 `https://你的用户名.github.io/my-workbench/` 即可。
   打开就是导航页，点卡片进对应工作台。

## 关于 screenwrite.html（编剧工作台本体）

该文件在你凌晨恢复的编剧工作台沙箱里，需要你从那个工作台导出 `.html` 源文件，
改名为 `screenwrite.html` 后放进本文件夹再一起上传即可。
（若暂时没有，导航页点它会 404，另外两个不受影响。）

## 注意事项

- 三个工作台都是单文件静态页，**数据保存在你访问所用浏览器的本地存储（localStorage）**。
  换浏览器 / 清缓存会看不到旧数据，重要数据记得用各自工作台的备份/导出功能留存。
- 想给某个工作台单独网址？直接访问对应文件名即可，例如
  `https://你的用户名.github.io/my-workbench/learning-dashboard.html`。
