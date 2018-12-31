---
title: "Automatic deploy previews for Merge Requests"
date: 2018-12-30T22:15:50-04:00
publishdate: 2018-12-30T22:15:50-04:00
anchor: automatic-deploy-previews-merge-requests
weight: 09
draft: false
---

Create a new Git branch:

`git checkout -b UglyTitles`

Silly CSS that we add to `custom.css`:

```css
.mdl-card__media h3 {
  // I set the color to red…
  color: red;
  // transform the text to uppercase…
  text-transform: uppercase;
}

// And our client wants some goofy emoji after each title. We add

.mdl-card__media h3:after {
  content: "💯🍌"
}
```

Update submodules:

`git submodule update`

Deleting the `UglyTitles` branch:

```shell
git checkout master
git branch -D UglyTitles
```
