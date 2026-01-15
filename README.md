# 2026 胖胖生日快乐 - 3D 互动贺卡

这是一个基于 Three.js 和 MediaPipe 的 3D 互动网页应用，支持手势控制、粒子特效和照片上传。

## 部署方法 (国内访问优化版)

由于 Vercel 的默认域名在中国大陆可能无法访问，推荐使用 **Surge** 或 **Netlify** 进行部署。

### 方案 A：使用 Surge 部署 (推荐，简单快速)

1. **打开终端**：在编辑器下方打开终端。
2. **运行命令**：
   ```bash
   npx surge
   ```
3. **按照提示操作**：
   - 输入邮箱和密码（如果是第一次，会帮您注册）。
   - `project path`: 默认是当前目录，直接回车。
   - `domain`: 系统会随机分配一个 `xxx.surge.sh` 的域名，您也可以自己修改成好记的名字（例如 `pangpang-birthday.surge.sh`），然后回车。
4. **完成**：复制终端显示的链接即可访问。

### 方案 B：使用 Netlify 部署

1. **运行命令**：
   ```bash
   npx netlify-cli deploy --prod
   ```
2. **按照提示操作**：
   - 登录 Netlify 账号。
   - 选择 `Create & configure a new site`。
   - `Publish directory`: 默认为 `.` (当前目录)，直接回车。
3. **完成**：终端会显示 `Website Draft URL` 和 `Website Live URL`，复制 Live URL 即可。

### 本地开发

由于使用了 ES Modules 和摄像头权限，直接双击打开 `index.html` 可能无法正常工作。建议使用本地服务器：

1. 使用 VS Code 的 **Live Server** 插件。
2. 或者在终端运行：`npx serve .`

## 功能特性

- **粒子倒计时**：支持中文的粒子汇聚效果。
- **手势控制**：通过摄像头识别手势（握拳、张开、捏合）控制 3D 场景。
- **照片上传**：支持上传本地照片并在 3D 蛋糕中展示。
- **黑金风格**：高端的 Bloom 辉光特效。

## 优化说明
已将所有 CDN 资源替换为国内访问速度更快的 `npm.elemecdn.com`，确保在中国大陆能流畅加载。
