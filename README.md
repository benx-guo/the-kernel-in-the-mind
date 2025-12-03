# The Kernel In The Mind

The Kernel In The Mind: Understanding Linux Kernel Before Code

Author: [moon-hee-lee](https://www.linkedin.com/in/moon-hee-lee)

这是一个使用 [mdbook](https://rust-lang.github.io/mdBook/) 构建的在线书籍项目。

## 📚 在线版本

访问 [GitHub Pages](https://bguo2.github.io/the-kernel-in-the-mind/) 查看在线版本。

## 🚀 本地开发

### 安装 mdbook

```bash
# 使用 cargo 安装（需要先安装 Rust）
cargo install mdbook

# 或者使用 Homebrew (macOS)
brew install mdbook
```

### 本地预览

```bash
# 启动本地服务器
mdbook serve

# 默认访问地址: http://localhost:3000
```

### 构建

```bash
# 构建静态网站
mdbook build

# 构建输出在 ./book 目录
```

## 📝 编辑内容

- 所有源文件在 `src/` 目录
- `src/SUMMARY.md` 定义了书籍的目录结构
- 编辑 Markdown 文件后，mdbook 会自动重新加载（使用 `mdbook serve` 时）

## 🔄 CI/CD

项目配置了 GitHub Actions，当推送到 `main` 分支时会自动：
1. 构建 mdbook
2. 部署到 GitHub Pages

## 📖 项目结构

```
.
├── book.toml          # mdbook 配置文件
├── src/               # 源文件目录
│   ├── SUMMARY.md    # 目录结构
│   └── *.md          # 章节文件
└── .github/
    └── workflows/     # CI/CD 配置
```

## 📄 License

This project is licensed under the [GNU General Public License v2.0](LICENSE) (GPL-2.0).
