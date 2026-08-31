# 招聘网站信息助手

## 使用

直接打开 `招聘网站信息助手.html` 即可使用。网页中的编辑内容默认只保存在当前浏览器；修改后请点击“保存修改”。

## 分享到非本地

这是一个纯静态网页，不需要服务器端程序。可以选择以下任一方式发布：

### GitHub Pages

本项目已包含 `index.html` 和 GitHub Actions 部署配置。推送到 `main` 分支后会自动发布到 GitHub Pages。

首次发布时，在 repository 的 **Settings → Pages → Build and deployment** 中选择 **GitHub Actions**。私有仓库的 Pages 功能取决于 GitHub 账号套餐；若账号不支持，需改用公开仓库或 Netlify。

### Netlify

在 Netlify 中选择 **Add new site → Deploy manually**，将包含 HTML 和 README 的文件夹拖入上传区域，即可获得公网链接。

## 导入与导出

- 支持导入 `.pdf`、`.txt`、`.md` 和本工具数据 `.json`。
- PDF 文本解析和 PDF 下载需要加载 CDN 组件；若网络不可用，TXT、Markdown、JSON 导入仍可使用，PDF 导出可改用浏览器打印并选择“另存为 PDF”。
- 导出文件名会自动生成 `Resume-YYYY-MM-DD.pdf` 或 `简历-YYYY-MM-DD.pdf`。

## 隐私

网页不会自动上传个人资料。公网地址只是静态页面地址，每个浏览器的编辑内容仍独立保存在本地 `localStorage` 中；不要把含有个人信息的导出文件上传到公开目录。
