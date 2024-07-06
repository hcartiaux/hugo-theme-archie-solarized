# Archie-solarized - Hugo theme

Archie-solarized is a minimal and clean theme for hugo with a markdown-ish UI.

Forked from [Ahtul Archie Theme](https://github.com/athul/archie) and converted to [Solarized color scheme](https://ethanschoonover.com/solarized/).

## Demo

[Check the Demo](https://hcartiaux.github.io/), I use this theme for my sysadmin notes :smile:

![](/images/theme.png)
![](/images/archie-dark.png)
## Feature
- Google Analytics Script
- Callouts
- Tags
- Auto Dark Mode(based on system theme)
- Dark/Light Mode toggle
- tl:dr; frontamatter
- Cache busting for CSS files
- Disqus Comments

## Installation
In your Hugo website directory, create a new folder named theme and clone the repo
```bash
$ mkdir themes
$ cd themes
$ git clone https://github.com/hcartiaux/hugo-theme-archie-solarized archie-solarized
```
Edit the `config.toml` file with `theme="archie"`
For more information read the official [setup guide](https://gohugo.io/installation/) of Hugo.

If you encounter any issues with Google Analytics, update Hugo to v0.125.0 or
later and make sure your using the latest version of the theme.

## Writing Posts
Create a new `.md` file in the *content/posts* folder
```yml
---
title: Title of the post
description:
date:
tldr: (optional)
draft: true/false (optional)
tags: [tag names] (optional)
toc: true/false (optional)
---
```

## Credits

Forked from [Ahtul Archie Theme](https://github.com/athul/archie), which is forked from [Ezhil Theme](https://github.com/vividvilla/ezhil) and Licensed under MIT License
Inspired by design of blog.jse.li

----

## Config Options

### Custom CSS
Custom CSS files can be included though the `customcss` config parameter.

Note: CSS files should be placed under the `assets` directory e.g. `assets/css/first.css`.

```toml
[params]
	customcss = ["css/first.css", "css/second.css"]
```


## Config of the Demo Site

```toml
baseURL = "https://example.com"
languageCode = "en-us"
title = "Archie-solarized"
paginate = 5
theme="archie-solarized"
copyright = "© H. Cartiaux"
pygmentsstyle = "monokai"
pygmentsStyle = "solarized-dark"
pygmentscodefences = true
pygmentscodefencesguesssyntax = true
[params]
    mode="toggle"
    useCDN=false
    subtitle = "Minimal and Clean [blog theme for Hugo](https://github.com/hcartiaux/hugo-theme-archie-solarized)"
    mathjax = false # enable MathJax support
    katex = true # enable KaTeX support

[[params.social]]
name = "GitLab"
icon = "gitlab"
url = "https://gitlab.com/hcartiaux/"

[[params.social]]
name = "GitHub"
icon = "github"
url = "https://github.com/hcartiaux/hugo-theme-archie-solarized"

[[params.social]]
name = "Linkedin"
icon = "linkedin"
url = "https://www.linkedin.com/in/hyacinthecartiaux/"

[[params.social]]
name = "Twitter"
icon = "twitter"
url = "https://twitter.com/hcartiaux/"

[[menu.main]]
name = "Home"
url = "/"
weight = 1

[[menu.main]]
name = "All posts"
url = "/posts"
weight = 2

[[menu.main]]
name = "About"
url = "/about"
weight = 3

[[menu.main]]
name = "Tags"
url = "/tags"
weight = 4
```
---

