---
title: "Install your new Hugo theme"
date: 2018-09-04T21:11:49-04:00
publishdate: 2018-09-04T21:11:49-04:00
anchor: install-your-new-hugo-theme
weight: 04
draft: false
---

**Note: If you're following along with the course, clone my fork of the theme to avoid issues.**

It's at https://github.com/tygerbytes/HugoMDL

The SSH url is: https://github.com/tygerbytes/HugoMDL.git

### clone method

`git clone --depth 1 https://github.com/tygerbytes/HugoMDL.git ./themes/HugoMDL`

Delete the `.git` directory:

Windows PowerShell: `rm --recurse --force .\themes\HugoMDL\.git`

Mac/Linux: `rm -rf ./themes/HugoMDL/.git`

### submodule method

`git submodule add https://github.com/tygerbytes/HugoMDL.git ./themes/HugoMDL`

Showing `.gitignore` from the command line:

`cat ./.gitignore`
