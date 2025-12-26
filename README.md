# 星火项目研究文档与资料

本仓库用于保存星火项目相关的研究内容与资料（PDF 与 Word 文档），并提供协作版 Markdown 文档以便评审与版本对比。

## 使用建议

- 小体积文档（<50MB）：可直接上传。
- 大体积或最终版文档：使用 Git LFS 跟踪（本仓库已配置建议）。
- 协作评审：建议把核心内容转为 Markdown（存放在 `docs/` 目录），便于逐行对比与讨论。

## 上传步骤

### 网页端（不走 LFS）
1. 仓库主页 → `Add file` → `Upload files`
2. 选择本地文件（如 `研究内容和意义.docx` 或 PDF）
3. 填写提交信息并提交

> 注意：网页端上传不会应用 Git LFS。若需 LFS，请使用本地 Git。

### 本地 Git（走 LFS）
1. 安装并初始化 LFS：`git lfs install`
2. 建议跟踪：`*.pdf`、`*.docx`���`*.doc`
3. 添加并推送（示例）：
   - `git add deliverables/研究内容和意义.docx`
   - `git commit -m "docs: add 研究内容和意义.docx"`
   - `git push`

## DOCX 转 Markdown（可选）
- 使用 Pandoc：
  - `pandoc -i "研究内容和意义.docx" -t gfm -o "docs/研究内容和意义.md"`

## 目录结构建议
- `docs/`：协作版 Markdown 文档与说明
- `assets/`：图片、插图与附属资源
- `deliverables/`：最终发布的 PDF/Word 版本
