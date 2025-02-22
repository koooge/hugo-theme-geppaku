![Deploy to github pages](https://github.com/koooge/hugo-theme-geppaku/workflows/Test/badge.svg)

Geppaku
=============================
Geppaku is bluish white theme for [Hugo](http://gohugo.io/).

Note that it is not in the "Seppuku".
I'm not Samurai.

Please check [https://koooge.github.io/hugo-theme-geppaku/](https://koooge.github.io/hugo-theme-geppaku/), if you are interested in this theme.

## Screenshot
### Index page
![list](https://github.com/koooge/hugo-theme-geppaku/blob/main/images/list.png)

### Post page
![post](https://github.com/koooge/hugo-theme-geppaku/blob/main/images/screenshot.png)

## Installation

```
$ mkdir themes
$ cd themes
$ git clone https://github.com/koooge/hugo-theme-geppaku hugo-theme-geppaku
```
See the Hugo documentation for more information.


## Config

Example of config.toml file:
```toml
baseurl = "http://your-site-here/"
languageCode = "en-us"
title = "your site title"
theme = "hugo-theme-geppaku"
googleAnalytics = ""
disqusShortname = ""
# enableRobotsTXT = true

[author]
    # If you want to display author information set these
    # This is Optional values
    name = "Your name"

    # Please set account ids
    # This is Optional values
    x_twitter = "your x id"
    linkedin  = "your linkedin id"
    github    = "your github id"
    tumblr    = "your tumblr id"
    bluesky   = "your bluesky id"

[params]
    [params.sharebutton]
        # If you want to display share buttons set these
        # This is Optional values
        x_twitter = true
        facebook  = true
        tumblr    = true
        # hatena   = true # hatena is Japanese social media
        google    = true
        pocket    = true
        # Please set id when you want to display facebook
        facebookAppId = "your app id"
        bluesky   = true

    [params.adsense]
        # If you want to display Google adsense set these
        # This is Optional values
        # 1. Create file written of the adsense tag into the directory "layouts/partials"
        # 2. Please set file path name omitted "layouts/partials"
        sidebar = "adsense/sidebar.html"
        content = "adsense/content.html"
```
You can delete optional parameter.
Please delete unnecessary parameter.

- :white_check_mark: [Multilingual Mode](https://gohugo.io/content-management/multilingual/)

### Post

Create markdown file:
```sh
hugo new post/2016/05/hello-hugo.md
```

Example of the markdown file:
```md
+++
date = "2016-04-30T16:44:45+09:00"
draft = false
title = "Hello Hugo!"
slug = "hello-hugo"
categories = ["tech"]
tags = [
  "hugo",
  "golang",
  ]
+++
Hello Hugo!
```

## Test

```sh
hugo server --configDir ./exampleSite/config --config ./exampleSite/config/test/config.toml --themesDir ./ --layoutDir ./layouts --contentDir ./exampleSite/content
```
