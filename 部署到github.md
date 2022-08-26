# 5.部署到github

### 5.1  构建书籍

首先，使用 gitbook build 将书籍内容输出到默认目录，也就是当前目录下的 _book 目录。

```
$ gitbook build
Starting build ...
Successfully built!

$ ls _book
GLOSSARY.html       chapter1            chapter2            gitbook             glossary_index.json index.html          search_index.json
```

### 5.2 创建 gh-pages 分支

```
git init //在_book目录
git add -A
git commit -m "Publish book"
git push -f 仓库地址.git master:gh-pages
```

书籍的内容已经上传到 GitHub 上，所以通过访问 ivanmao714.github.io/Gitbook就可以阅读 test 这本书了！
