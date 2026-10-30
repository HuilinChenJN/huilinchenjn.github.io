# Huilin Chen 学术主页

基于 Minimal Light，保留模板原有布局、字体与深浅色模式。

## 日常维护
- `_config.yml`：姓名、身份、单位、邮箱、Scholar 链接。添加邮箱时加一行 `email: your-address`。
- `index.md`：个人介绍与研究方向。
- `_data/publications.yml`：论文列表，按显示顺序排列。复制一个论文条目后修改即可，保持缩进一致。
- 照片：上传到 `assets/img/profile.jpg`，在 `_config.yml` 添加 `avatar: ./assets/img/profile.jpg`。
- 简历：上传到 `assets/files/cv.pdf`，在 `_config.yml` 添加 `cv_link: assets/files/cv.pdf`。

## 发布到 GitHub Pages
1. 在 HuilinChenJN 账号新建公开仓库 `HuilinChenJN.github.io`。
2. 上传本目录内全部文件，保留以 `_` 开头的目录；不要额外嵌套一层文件夹。
3. Settings → Pages → Deploy from a branch → main → /(root) → Save。
4. 等待构建完成，访问 https://huilinchenjn.github.io/ 。

## 内容来源与维护
个人介绍、教育经历、工作经历和学术服务来自本人提供的英文简历。
页面列出 8 篇论文：Google Scholar 当前有 7 篇，另有简历列出的 Neural Networks 论文。
LLM-ASAR 已由本人确认录用，并与 Scholar 的期刊和年份核对（ACM TORS, 2026）。
TOIS 论文的作者与年份按简历及已核对 DOI 保留；Scholar 条目存在差异。
照片从简历原样提取；简历 PDF 原样复制到 `assets/files/Huilin_Chen_CV.pdf`。
未来更新照片请替换 `assets/img/profile.jpg`；更新简历请替换上述 PDF。
未配置引用统计自动同步；Scholar 链接可查看实时信息。
未启用模板作者的统计账号、示例新闻或个人域名。

## 本地构建（可选）
安装兼容 GitHub Pages 的 Ruby 后，运行 `bundle install` 和 `bundle exec jekyll serve`。


本次更新：新增本人确认录用的 TOIS 论文（作者名单、年份和链接待补），共 9 篇；使用两份框架 PDF 转出的图片及用户提供 PNG，为 3 篇论文恢复图文排版和会议标签。原始输入文件未修改。桌面查看通过；390px 手机视口无横向溢出（内容宽 375px），三张配图均正常加载。新增样式 assets/css/custom.css。
