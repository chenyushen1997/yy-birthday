# 2026 胖胖生日快乐 - 3D 互动贺卡

这是一个基于 Three.js 和 MediaPipe 的 3D 互动网页应用，支持手势控制、粒子特效和照片上传。

## 部署方法：GitHub Pages (详细步骤)

GitHub Pages 更加稳定，且域名看起来更正式。

**步骤 1：创建仓库**
1. 登录 [GitHub](https://github.com)。
2. 点击右上角的 **+** 号 -> **New repository**。
3. Repository name 输入 `birthday-2026` (或者其他你喜欢的名字)。
4. 确保选择 **Public**。
5. **不要**勾选 "Add a README file" (因为本地已经有了)。
6. 点击 **Create repository**。

**步骤 2：推送代码**
在编辑器下方的终端中，依次运行以下命令（将 `你的GitHub用户名` 替换为你真实的用户名）：

```bash
# 关联远程仓库
git remote add origin https://github.com/你的GitHub用户名/birthday-2026.git

# 推送代码
git push -u origin main
```

**步骤 3：开启 Pages**
1. 回到 GitHub 仓库页面，点击顶部的 **Settings** (设置)。
2. 在左侧边栏找到 **Pages**。
3. 在 **Build and deployment** 下的 **Source** 选择 `Deploy from a branch`。
4. 在 **Branch** 选项中，选择 `main` 分支，文件夹选择 `/ (root)`，然后点击 **Save**。
5. 等待几分钟，刷新页面，你会在顶部看到生成的链接（例如 `https://你的用户名.github.io/birthday-2026/`）。

## 功能特性

- **微信引导**：自动检测微信环境，提示用户跳转浏览器，避免白屏或被拦截。
- **粒子倒计时**：支持中文的粒子汇聚效果。
- **手势控制**：通过摄像头识别手势（握拳、张开、捏合）控制 3D 场景。
- **照片上传**：支持上传本地照片并在 3D 蛋糕中展示。
