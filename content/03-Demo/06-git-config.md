---
title: "3-6 Configure project to use Git"
anchor: "demo_configure_project_git"
weight: 35
---

Configure global Git user settings
```
git config --global user.name “Your name" 
git config --global user.email “email@domain.com"
```

Initialize git and upload your files
```
git init
git remote add origin git@gitlab.com:<YOUR-USER-NAME>/<YOUR-REPO>.git 
git add . git commit -m "Initial commit“
git push -u origin master
```

Configure SSH keys
* https://gitlab.com/profile/keys 
* https://gitlab.com/help/ssh/README#generating-a-new-ssh-key-pair
