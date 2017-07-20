# Clexy

> Clexy ( Customized-Flexy ) is a modern reponsive theme for [Hexo](https://hexo.io/).

## Demo

You can see the theme in action on my [website](https://mkkhedawat.com/).

## Setting up

#### In Console
```
$ git clone https://github.com/mkkhedawat/clexy themes/clexy
$ yarn remove hexo-renderer-ejs
$ yarn add hexo-renderer-jade
$ yarn add hexo-prism-plugin
```
#### In root's _config.yml :

- Change your `theme` variable to `clexy`
- Add `prism_plugin` options
```
prism_plugin:
  mode: 'preprocess'    # realtime/preprocess
  theme: 'default'
  line_number: false    # default false
```
- Make sure that default code `highlight` plugin is disabled.
```
highlight:
  enable: false
```

## Post Variables

- Add the `intro` variable to your YAML in your Markdown file.
- Comments can be toggled with the `comments` boolean variable.
- Add tag to post using `tags` variable.

```md
---
title: 'Title Name'
date: 2017-06-01 21:56:56
tags:
- tag1
- tag2
intro : 'Enter intro here to display on home page'
comments: false
---
```

## Booting up blog
```
$ hexo new page "articles"
$ hexo new page "author"
$ hexo new post "Title-1"
$ hexo new post "Title-2"
```
Add content and post variables to both posts, Later
```
$ hexo clean
$ hexo server
```
Open browser and navigate to http://localhost:4000/

## License

MIT © [Manish Kumar Khedawat](http://mkkhedawat.com)
