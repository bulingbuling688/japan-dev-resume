# 对日开发简历

## 项目简介

这是一个面向对日开发岗位的 LaTeX 简历项目，使用标准 `article` 模板与轻量样式封装，便于后续持续修改、导出与版本管理。

## 主要内容

- `main.tex`：简历主文件
- 顶部信息区、教育背景、专业能力、项目经历、自我评价等模块
- 支持 PDFLaTeX 与 XeLaTeX/CTeX 两种中文编译路径

## 使用方式

### 编译

推荐使用 XeLaTeX：

```bash
latexmk -xelatex -interaction=nonstopmode -halt-on-error -file-line-error main.tex
```

如果使用 PDFLaTeX，请确保环境支持 `CJKutf8`。

## 文件说明

- `main.tex`：当前对日开发方向简历源码
- `avatar1.jpg`：可选头像文件；不存在时会自动显示占位框
- `.gitignore`：忽略中间编译产物

## 维护说明

- 当前仓库仅用于 GitHub 版本管理，不连接 Overleaf
- 后续可直接在本项目基础上继续修改对日开发方向简历
- 如果需要区分不同岗位版本，建议基于当前版本新建分支维护
