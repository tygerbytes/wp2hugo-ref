---
title: "3-9 Deploy site to GitLab Pages"
anchor: "demo_deploy_gitlab_pages"
weight: 35
---

pull in changes made in Gitlab:
```
git pull
```

"stash" unsaved changes before running `git pull`:
```
git stash
git pull
git stash pop
```

Install Node.js from [https://nodejs.org/en/download/current/](https://nodejs.org/en/download/current/) 

Installing `http-server`:
```
npm install http-server -g
```

Running web server from `./public`:
```
hugo
http-server
```

Delete the public directory:

Windows PowerShell:
```
rm -recurse -force public
```

Mac/Linux:
```
rm -rf ./public
```
