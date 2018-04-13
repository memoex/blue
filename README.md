# Blue

A responsive theme inspired by documentation site of Bootstrap for Hugo blog framework.

## Demo

Blog demo: https://memoex.github.io

![](https://i.imgur.com/KD1PetE.png)

## Features

- [x] Responsive.
- [x] Nice and convenient sidebar.
- [x] TOC (table of content).
- [x] Syntax Highlighting.
- [x] Copy code block to clipboard with single click.
- [x] MathJax.
- [x] Show images with fancybox.
- [x] Beautiful [fonts](http://localhost:1313/note/tech/css/) and [material color](https://material.io/guidelines/style/color.html#color-color-palette).
- [x] Disqus comment.
- [x] Tags.
- [ ] Blog searching.


## Quick start

### Installation

First you need to have hugo installed and use hugo to create a new website. See the [Quick Start](http://gohugo.io/getting-started/quick-start/) if hugo is new for you.

After you have a new hugo website, the directory structure must look like this:

```
.
├── archetypes
├── config.toml
├── content
├── data
├── layouts
├── static
└── themes
```

Then move to `themes` folder. If you don't have this folder, just create one.

Run the commands below to install `blue` theme:

``` sh
git clone https://github.com/memoex/blue.git
```

Then you could use this theme in two ways.

One is to pass the `-t` flag:

- building your site for deployment: `hugo -t blue`
- starting a local server at http://localhost:1313 (default): `hugo server -t blue`

The other one is to change your configuration file `config.toml`. Change the value of `theme` as below:

```
theme = "blue"
```

Then you don't need an extra `-t` flag anymore.

### Configuration

Below is my `config.toml`, you can replace the values with your information.

``` toml
baseurl = "https://memoex.github.io/"
DefaultContentLanguage = "en"
title = "Mr.Blue"
theme = "blue"
metaDataFormat = "yaml"

[Params]
  subtitle = "Mr.Blue doesn't have a good memory."
  favicon = "/favicon.ico"                          # when build website, the files under `/static` will be moved to `/`

[Author]
  name = "Mr.Blue"
  website = "https://memoex.github.io"
  email = "silverhugh.77@gmail.com"
  github = "blue-fatty"

[[menu.main]]
    identifier = "note"
    name = "Note"
    url = "/note/"                                  # url should end with `/` to make highlighting of navigation bar works
    weight = 2                                      # small weight go left, large weight go right

[[menu.main]]
    identifier = "project"
    name = "Project"
    url = "/project/"
    weight = 2

[[menu.main]]
    identifier = "tags"
    name = "Tags"
    url = "/tags/"
    weight = 2

[[menu.main]]
    identifier = "about"
    name = "About"
    url = "/about/"
    weight = 3
```
