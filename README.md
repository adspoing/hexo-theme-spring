# Spring

A theme for [Hexo].

- [Preview](http://www.springwon.cn)

## Installation

### Install

``` bash
$ git clone https://github.com/adspoing/hexo-theme-spring.git themes/spring
```

**Spring requires Hexo 2.4 and above.**

### Enable

Modify `theme` setting in `_config.yml` to `spring`.

### Update

``` bash
cd themes/spring
git pull
```

## Configuration

``` yml
# Header
menu:
  主页: /
  所有文章: /archives
  随笔: /tags/随笔
social:
  zhihu: 
  facebook: 
  github: 

# Content
excerpt_link: Read More
fancybox: true

# Sidebar
sidebar: right
widgets:
- category
- tag
- tagcloud
- archives
- recent_posts

# Miscellaneous
google_analytics:
favicon: /favicon.png
twitter:
google_plus:

#Personal
avatar: 
```

- **menu** - Navigation menu
- **excerpt_link** - "Read More" link at the bottom of excerpted articles. `false` to hide the link.
- **fancybox** - Enable [Fancybox]
- **sidebar** - Sidebar style. You can choose `left`, `right`, `bottom` or `false`.
- **widgets** - Widgets displaying in sidebar
- **google_analytics** - Google Analytics ID
- **favicon** - Favicon path
- **twitter** - Twiiter ID
- **google_plus** - Google+ ID


## Features

### Fancybox

Landscape uses [Fancybox] to showcase your photos. You can use Markdown syntax or fancybox tag plugin to add your photos.

```
![img caption](img url)

{% fancybox img_url [img_thumbnail] [img_caption] %}
```

## Development

### Requirements

- [Grunt] 0.4+
- Hexo 2.4+

### Grunt tasks

- **default** - Download [Fancybox] and [Font Awesome].
- **fontawesome** - Only download [Font Awesome].
- **fancybox** - Only download [Fancybox].
- **clean** - Clean temporarily files and downloaded files.

[Hexo]: https://hexo.io/
[Fancybox]: http://fancyapps.com/fancybox/
[Font Awesome]: http://fontawesome.io/
[Grunt]: http://gruntjs.com/
