---
title: "Getting Started With Hugo"
date: 2023-01-17T10:10:23-06:00
draft: true
---

0. Initialize the site

```shell
hugo new site course_forge
cd course_forge
git init
git add .
git commit -m "Initialized Hugo Site"
```

2. Add this page.

```shell
hugo new notes/getting-started-with-hugo.md
```

3. Add HugoTex Theme

```shell
git clone git@github.com:kaisugi/HugoTeX.git themes/HugoTeX
rm -rf themes/HugoTex/.git
echo "theme = 'HugoTex'" >> config.toml
git add .
git commit -m "Add HugoTex theme: git@github.com:kaisugi/HugoTeX.git"
```

4. Launch and view site

```shell
open http://localhost:1313 && hugo server -wD --navigateToChanged
```
