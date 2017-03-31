---
layout: post
title:  "How to host Angular application on GitHub Pages"
date:   2017-03-31 15:26:55 -0400
categories: angular github
published: true
---
To host Angular application on GitHub Pages use [angular-cli-ghpages](https://github.com/angular-buch/angular-cli-ghpages)

> Note: you have to create the **dist** folder in before (e.g. `ng build --prod`)

```
ng build --prod --base-href "https://USERNAME.github.io/REPOSITORY/"
ngh
```

If you have a custom domain you should use `http` instead

```
ng build --prod --base-href "http://YOURDOMAIN.com/REPOSITORY/"
ngh
```

There might be a problems with routing. If so check [this FAQ](https://github.com/angular-buch/angular-cli-ghpages/wiki/FAQ#why-is-the-routing-not-working-correctly-on-hard-reload-specific-to-github-pages-only)