## 🚀 GitHub Pages 部署指南

### 方式一：GitHub 网页上传（最快，2分钟完成）

1. 打开 https://github.com/new ，创建新仓库：
   - Repository name: `shipping-analytics-v1`
   - 描述：`航运与物流公司可视化分析V1.0`
   - Public
   - **不要**勾选 Add a README file
   - 点击 Create repository

2. 进入新仓库页面，点击 "uploading an existing file"
3. 将以下文件拖入上传区：
   - `index.html`（主文件）
4. Commit message 填写：`feat: 航运与物流公司可视化分析 V1.0`
5. 点击 Commit changes

6. 进入仓库 **Settings → Pages**：
   - Source 选择 `Deploy from a branch`
   - Branch 选择 `main`，文件夹选 `/ (root)`
   - 点击 Save

7. 等待约 2-3 分钟，访问：
   👉 https://caijiazongz.github.io/shipping-analytics-v1/

---

### 方式二：命令行推送（需要PAT）

```bash
# 在 GitHub → Settings → Developer settings → Personal access tokens → Fine-grained tokens
# 创建一个新 Token，勾选 Contents: Read and write

cd C:\Users\caiji\WorkBuddy\2026-06-09-task-4\shipping-dashboard

# 推送到新仓库（替换YOUR_PAT为你的token）
git remote set-url origin https://caijiazongz:YOUR_PAT@github.com/caijiazongz/shipping-analytics-v1.git
git push -u origin main
```

---

### 本地文件位置
`C:\Users\caiji\WorkBuddy\2026-06-09-task-4\shipping-dashboard\index.html`
