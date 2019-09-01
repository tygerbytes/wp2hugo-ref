---
title: "netlify.toml: Branch-specific deploy settings"
date: 2018-12-31T05:20:50-04:00
publishdate: 2018-12-31T05:20:50-04:00
anchor: netlify-more-control-netlify-toml
weight: 11
draft: false
---

* [Netlify continuous deployment: deploy contexts](https://www.netlify.com/docs/continuous-deployment/#deploy-contexts)

Creating the branch and pushing it to GitLab:

```shell
git checkout -b draft-post-preview
git push --set-upstream origin draft-post-preview
```

```toml
# netlify.toml
[build]
  command = "hugo"
  publish = "public"

# Branch Deploy context: all deploys that are not from a pull/merge request or
# from the Production branch will inherit these settings.
[context.branch-deploy]
  command = "hugo -D"

# Specific branch context: all deploys from this specific branch will inherit
# these settings.
[context.draft-post-preview] # 'staging' is a branch name
  command = "hugo -D"
```
