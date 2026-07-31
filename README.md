# 刘继凡工作台 · 上线指南（GitHub Pages）

目标：把工作台放到 GitHub 上，凡哥手机浏览器打开就是**每天自动最新**的，再也不用覆盖手机文件。

---

## 一、建 GitHub 仓库（你做，2 分钟）
1. 打开 https://github.com → 右上角 ➕ → **New repository**
2. 仓库名填：`liujifan-workbench`
3. 选 **Public**
4. 其余别动 → 点 **Create repository**

## 二、把库推上去（二选一）

### 方式A：给我 Token，我直接推（最省事，推荐）
1. GitHub → 右上角头像 → **Settings** → **Developer settings** → **Personal access tokens** → **Tokens (classic)** → **Generate new token**
2. 勾 **repo** 权限，有效期选 90 天或 No expiration
3. 复制生成的 token（只显示一次）发给我
4. 再把仓库地址发我：`https://github.com/你的用户名/liujifan-workbench.git`
→ 我配好 remote 并 push，以后每天自动更新，你零操作。

### 方式B：你自己推（电脑装了 git）
在「刘继凡工作台」文件夹里右键 **Git Bash**，粘贴：
```
git remote add origin https://github.com/你的用户名/liujifan-workbench.git
git branch -M main
git push -u origin main
```

## 三、开 Pages（你做，1 分钟）
1. 进仓库 → **Settings** → **Pages**
2. Source 选 **Deploy from a branch** → Branch 选 **main** → 目录 **/root** → **Save**
3. 等 1–2 分钟，访问：`https://你的用户名.github.io/liujifan-workbench/mobile.html`

## 四、手机上用
1. 手机浏览器打开上面的 URL
2. 右上角 ⋯ → **添加到主屏幕** → 名字「刘继凡工作台」
3. 以后点图标就是 App，**每天自动最新**（我 08:00 爬热点写库 + 自动 push 到 GitHub，Pages 立刻生效）

## 五、文件说明（本地库已 commit 就绪）
- `index.html` —— 桌面版（深色）
- `mobile.html` —— 移动版（浅色，已支持「远程数据源」设置）
- `workbench-data.js` —— 抖音爆款热点数据，每天 08:00 自动刷新
- 三个文件已在本地 git 仓库首次提交中

## 六、备选：不想用 GitHub？
也可发我 Gitee（码云）仓库地址，走 Gitee Pages（国内访问更稳）。或让我用 CloudStudio 部署国内 URL（偶发超时，需重试）。GitHub Pages 最稳、最永久。
