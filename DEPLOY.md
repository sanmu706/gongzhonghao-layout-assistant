# 部署到 GitHub Pages

## 推荐方式：仓库根目录部署

1. 在 GitHub 新建一个公开仓库，例如：

   `gongzhonghao-layout-assistant`

2. 上传当前文件夹内的所有文件到仓库根目录。

   也就是说，仓库根目录应该直接包含：

   - `index.html`
   - `README.md`
   - `DEPLOY.md`
   - `.nojekyll`
   - `.gitignore`
   - 截图图片文件

3. 进入仓库的 `Settings`。

4. 打开左侧 `Pages`。

5. 在 `Build and deployment` 中选择：

   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`

6. 保存后等待 1-2 分钟。

7. GitHub 会生成访问链接，格式通常是：

   `https://你的用户名.github.io/gongzhonghao-layout-assistant/`

把这个链接发给其他用户，对方打开后即可直接使用。

## 常见问题

### 为什么不是直接发 GitHub 仓库链接？

`https://github.com/用户名/仓库名` 是代码仓库页面，不是工具页面。

用户真正使用的链接应该是 GitHub Pages 生成的：

`https://用户名.github.io/仓库名/`

### 可以私有仓库部署吗？

GitHub Pages 对私有仓库的支持取决于账号和组织权限。为了方便分享，建议使用公开仓库。

### 是否需要安装依赖？

不需要。当前工具只有一个 `index.html`，没有构建步骤，也没有后端服务。

### 更新功能后如何重新发布？

修改文件并提交到 `main` 分支后，GitHub Pages 会自动重新部署。

