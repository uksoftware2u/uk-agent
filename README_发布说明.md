# UK Agent Solution · GitHub Pages V4

## 本次交付状态

文件已生成并完成本地检查，**尚未创建 GitHub 仓库、上传或启用 Pages，也没有取得已上线网址**。
当前连接核对到的 GitHub 登录名为 `uksoftware2u`。本次可用 GitHub 操作仅提供读取；没有可用的创建仓库、提交文件或配置 Pages 的操作。本交付未修改任何既有仓库。

此包基于 BlueMotion V3：保留头像、蓝色能量动画、中英文切换及 12 个行业流程，更新咨询表单以支持纯静态托管。

## 最少文件上线

`index.html` 已包含图片、CSS 和 JavaScript。没有需要安装的依赖，没有构建命令，不必另外上传原 V3 的各个 JS / CSS 文件。
`.nojekyll` 为空文件，用于关闭 Jekyll 处理。

### 1. 创建一个独立仓库

在 GitHub 使用你要发布的账号，选择 New repository。

- Owner：本次核对账号为 `uksoftware2u`，也可使用你自己有管理权的其他账号。
- Repository name：建议 `uk-agent-solution`。
- 若账号使用 GitHub Free，选择 Public；源码、头像及公开销售号码都会公开，请不要混入客户资料或密钥。
- 打开 Add README，然后 Create repository。
- 不要把这个网站混进现有的维修系统代码仓库。

### 2. 上传网页

打开刚建的仓库，在 Code 页面选择 Add file → Upload files。
上传本压缩包里的 `index.html` 和 `.nojekyll` 到仓库根目录，再提交到 `main`。
**不要只上传 ZIP；不要把 index.html 放进多一层文件夹。**
若文件管理器隐藏 `.nojekyll`，可以在 GitHub 的 Add file → Create new file 建立同名空文件。此站也没有额外需 Jekyll 处理的页面。

### 3. 开启 GitHub Pages

打开仓库 Settings → Pages → Build and deployment：

```
Source: Deploy from a branch
Branch: main
Folder: / (root)
```

点击 Save，查看 Actions 中的 Pages 部署结果，再回 Settings → Pages 点击 Visit site。
官方说明更新可能需要最多约 10 分钟；以后台实际部署状态为准。

如果 Owner 设为 `uksoftware2u`、仓库名设为 `uk-agent-solution`，发布成功后的预计地址格式为：

```
https://uksoftware2u.github.io/uk-agent-solution/
```

这是计划地址，**不是已经创建或验证的在线网址**。使用其他账号或仓库名时，地址也不同。

## WhatsApp 咨询

主要按钮：整理资料并打开 WhatsApp / Prepare inquiry & open WhatsApp。
接收目标：`60127479966`（012-7479966）。

字段包括姓名、公司、行业、联系电话、电邮、现有系统、完整需求、页面语言、来源和联系同意状态。
原始需求不被翻译或改写；未填写选填项显示为“未填写 / Not provided”。

点击网页主按钮仅整理草稿并尝试打开 WhatsApp。**客户仍需在 WhatsApp 内点击发送；网页不能确认送达。**
支持先预览、复制全部资料、再次打开 WhatsApp 和只打开对话后粘贴。较长信息显示备用提示，不自动截断内容。
网页不会在打开 WhatsApp 后清空输入，不调用 AI 模型，不调用真实 MCP / AutoCount，不发送表单 POST 请求。
旧 Netlify Forms 和旧托管网址已移除；隐私说明同步更新。

## 上线后的实际验收

用手机和电脑分别打开真实的 Pages 地址：

1. 头像、蓝色光流、暂停/模式切换以及中英切换正常。
2. 12 行业流程可切换；行业咨询预填正确。
3. 使用非敏感测试资料填写表单，核对 WhatsApp 草稿内所有字段完整，目的号码正确。
4. 客户按下 WhatsApp 发送后，在销售手机确认收到。这一步尚未在本交付中执行。
5. 确认仓库、网页中没有客户资料、密码、API Key 或个人测试资料。

## 用途和隐私限制

GitHub Pages 是静态网站托管，不会在服务器运行 AI Agent、MCP、数据库或会计后台。
GitHub 官方明确限制把 Pages 作为运行在线业务、电商、主要促成商业交易或提供商业 SaaS 的免费托管。
本网页具有业务咨询与获客用途；不能仅因没有在线支付，就保证符合该限制。正式商业推广前应向 GitHub 确认适用范围；必要时保留 GitHub 做源码管理，把商业网站部署到允许该用途的托管服务。

GitHub Pages 会记录访客 IP 用于安全目的。表单草稿不持久化保存；语言偏好仍在访客浏览器本地保存。WhatsApp 处理的数据适用 WhatsApp 自身条款和隐私政策。
本次没有购买域名，没有执行任何付费升级。

## 本地检查

`QA_REPORT.json` 记录了 72 项检查结果：全部通过。
检查方式为将 HTML 注入 Chromium 后测试交互；运行环境策略阻止直接 file:// 导航，因此没有在浏览器中验证文件网址导航或真实 GitHub Pages 托管。
WhatsApp 打开请求在测试中被拦截，**没有发出真实消息**。剪贴板备用分支使用了测试替身，真实系统剪贴板访问仍取决于访客浏览器权限。
同一视窗、同一冻结动画时点下，V3 与 V4 首页截图逐像素相同。原动画 JS 和 neural.css 未改变。

## 官方参考（2026-09-09 核对）

- 创建 Pages：https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- 发布来源设置：https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- 上传文件：https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository
- Pages 服务及数据说明：https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages
- 用途与资源限制：https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits
