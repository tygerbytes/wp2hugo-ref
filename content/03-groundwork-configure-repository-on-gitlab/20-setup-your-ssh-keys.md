---
title: "20 Setup your SSH keys"
date: 2018-09-04T21:11:47-04:00
publishdate: 2018-09-04T21:11:47-04:00
anchor: 20-setup-your-ssh-keys
weight: 40
draft: false
---

``` bash
ssh-keygen -t rsa -C "your.email@example.com" -b 4096
cat ~/.ssh/id_rsa.pub | clip
```

More information: https://docs.gitlab.com/ee/ssh/README.html
