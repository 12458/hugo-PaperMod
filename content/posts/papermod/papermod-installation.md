---
title: "Papermod - Installation"
date: 2020-09-15T11:30:03+05:30
series: ["PaperMod"]
weight: 1
aliases: ['/papermod-installation']
tags: ['PaperMod']
author: "Aditya Telange"
showToc: true
TocOpen: true
---

## Guide

Follow [this](https://gohugo.io/getting-started/quick-start/) guide to setup hugo and create a new site.
Make sure you install latest version of `hugo`(>=0.57.1).

After you have created a new site, at [Step 3](https://gohugo.io/getting-started/quick-start/#step-3-add-a-theme) follow the steps:

Inside the folder of your Hugo site, run:

> ```console
> git clone https://github.com/adityatelange/hugo-PaperMod themes/hugo-PaperMod --depth=1
> ```
> > Updating theme :
> > ```console
> > cd themes/hugo-PaperMod
> > git pull
> > ```
> >

**or** you can use as [submodule](https://www.atlassian.com/git/tutorials/git-submodule) with
>
> ```console
> git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/hugo-PaperMod
> ```
> > Updating theme with submodule :
> > ```console
> > git submodule update --remote --merge
> > ```
> >
Then change in `config.yml`:
>
```yml
theme: "hugo-PaperMod"
```

Example Site Structure is present here: [exampleSite](https://github.com/adityatelange/hugo-PaperMod/tree/exampleSite/)

---

### Sample `config.yml`

```yml
baseURL: 'https://examplesite.com'
title: ExampleSite
paginate: 5
theme: hugo-PaperMod

enableRobotsTXT: true
buildDrafts: false
buildFuture: false
buildExpored: false

googleAnalytics: UA-123-45

minify:
  disableXML: true
  minifyOutput: true

params:
  env: production # to enable google analytics, opengraph, twitter-cards and schema.
  title: ExampleSite
  description: 'ExampleSite's description'
  author: Me

  images: "<link or path of image for opengraph, twitter-cards>"

  ShowReadingTime: true
  ShowShareButtons: true
  comments: false
  defaultTheme: auto
  disableThemeToggle : false
  disableSpecial1stPost : false

  # profile-mode
  profileMode:
    enabled: false # needs to be explicitly set
    title: ExampleSite
    # imageUrl: '<img location>'
    # imageTitle: my image
    buttons:
      - name: Posts
        url: posts
      - name: Tags
        url: tags

  # home-info mode
  homeInfoParams:
    Title: "Hi there \U0001F44B"
    Content: Welcome to my blog

  socialIcons:
    - name: twitter
      url: 'https://twitter.com/'
    - name: stackoverflow
      url: 'https://stackoverflow.com'
    - name: github
      url: 'https://github.com/'


  analytics:
    google:
      SiteVerificationTag: "XYZabc"
```

---

### Sample `Page.md`

```yml
---
title: "My 1st post"
date: 2020-09-15T11:30:03+00:00
weight: 1
aliases: ['/first']
tags: ['first']
author: "Me"
showToc: true
TocOpen: false
draft: false
hidemeta: false
disableShare: false
cover:
  image: '<image path/url>'
  alt: '<alt text>'
  caption: '<text>'
comments: false
---
```

---

###  [Papermod - Features](../papermod-features)
###  [Papermod - How to Guide](../papermod-how-to-guide)
###  [Papermod - Icons](../papermod-icons)