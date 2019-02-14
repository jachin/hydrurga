# Hydrurga

## A Hugo Theme

**Based on the [hugo-primer](https://github.com/qqhann/hugo-primer) theme.**

## Installation
Clone to your theme directory:
```terminal
$ git clone https://github.com/jachin/hydrurga.git themes/hydrurga

$ hugo server --theme=hydrurga
```

## Usage

#### config.toml
You can configure Hydrurga behavior with these params in your blog's `config.toml`. Shown are defaults and most recommended configs.

That being said, below is all recommended configurations.
```config.toml
# config.toml

baseURL = "https://your_web_site"
title = "Your Blog"
theme = "hugo-primer"
summaryLength = 70
# Code pen
pygmentsCodeFences = true
pygmentsUseClasses = true
googleAnalytics = "<Your Tracking Code>"

[frontmatter]
# update sitemap.xml's lastmod datetime by file change time, instead of git.
lastmod = ["lastmod", ":fileModTime", ":default"]

[params]
description = "Describe what your web page is about"
twitter = "your_twitter_id"
# You can use favicon by addin them manually.
useIcon = true
useTwitterCard = true

shareTo = ["Twitter", "Hatena", "Facebook", "Pocket"]
```

## Contributing
Issues and PRs are welcome.

## License
MIT
