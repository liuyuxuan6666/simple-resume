# LaTeX Resume Template (Single-Column, Engineering Style)
# LaTeX 简历模板（单栏 · 工程师风格）

This repository provides a **clean, single-column LaTeX resume template** designed for:
- Software / Computer Engineering roles
- Internet / Tech companies
- High-density, one-page–friendly resumes
- Linux / WSL users (XeLaTeX)

本仓库提供一份 **朴素、工程化、单栏 LaTeX 简历模板**，适用于：
- 计算机 / 软件 / 工程技术岗位
- 互联网与科技公司
- 内容密集、可压缩至一页
- Linux / WSL 环境（基于 XeLaTeX）

---

## Features / 特性

- Single-column layout, ATS-friendly  
- Density control (comfortable / compact / one-page)  
- Fully configurable via variables at the top of the source  
- Chinese & English mixed typesetting (XeLaTeX + xeCJK)  
- No icons, no colors, black & white only  

- 单栏结构，利于 ATS / 系统筛选  
- 页面密度可调（舒适 / 紧凑 / 极限一页）  
- 所有关键参数集中在源码顶部，像“配置文件”一样可维护  
- 原生支持中英混排  
- 纯黑白，无图标、无花哨样式  

---

## Environment Setup (Ubuntu)
## 环境配置（以 Ubuntu 为例）

> Tested on Ubuntu 20.04 / 22.04  
> 在 Ubuntu 20.04 / 22.04 上验证通过

### 1. Install TeX Live (XeLaTeX)
### 1. 安装 TeX Live（包含 XeLaTeX）

```bash
sudo apt update
sudo apt install -y texlive-xetex \
                    texlive-latex-recommended \
                    texlive-latex-extra \
                    texlive-fonts-recommended \
                    texlive-fonts-extra
```

---

### 2. Install Chinese Fonts (Recommended)
### 2. 安装中文字体（推荐）

```bash
sudo apt install -y fonts-noto-cjk
```

---

### 3. (Optional) WSL Users
### 3.（可选）WSL 用户说明

For WSL users, fonts installed in Windows are **not automatically available**.  
It is recommended to install fonts directly inside WSL.

---

## Compile the Resume
## 编译简历

```bash
xelatex resume.tex
```

Compile twice if needed:

```bash
xelatex resume.tex
xelatex resume.tex
```

---

## Configuration Knobs
## 关键配置说明

### Density / 页面密度
```tex
\newcommand{\DefaultDensity}{2}
```

1 = 舒适  
2 = 紧凑（推荐）  
3 = 极限一页  

### Body Font / 正文字号
```tex
\newcommand{\DefaultBodyFont}{2}
```

---

## License / 许可

Free for personal and educational use.
