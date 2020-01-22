# Gixx-web Static Website 

This is the Jekyll and architecture source code of the [gixx-web.com](https://www.gixx-web.com) website. 

## 1. License

The writings under the [_posts](_posts) folder and the image assets are protected by copyright, the rest is free for learning and using.

## 2. Usage

```
docker run --name gixxweb --volume="${PWD}:/srv/jekyll" -p 4002:4000 -it jekyll/jekyll:3.8 bash

jekyll serve -w --drafts --force_poll
```
