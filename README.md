# TapMe.plus Site Publish

Official Jekyll website for TapMe.plus.

Target domains:

- https://www.tapme.plus
- https://tapme.plus

Related project:

- Web game: https://web.tapme.plus
- Web publish repository: https://github.com/wanmeixx/tapme-plus-web-publish
- Source game repository: https://github.com/wanmeixx/TapMe-1-Godot

Cloudflare Pages settings:

- Framework preset: Jekyll
- Build command: `bundle exec jekyll build`
- Build output directory: `_site`
- Cloudflare builds `_site` from the Beautiful Jekyll source. The generated `_site` directory is not committed.

This site is based on Beautiful Jekyll and includes:

- Lightweight homepage with direct play links
- Blog posts under `_posts`, rendered through Beautiful Jekyll's post and home layouts
- News items under `_news`
- Automatic `/sitemap.xml` from `jekyll-sitemap`
- Privacy policy at `/privacy/`
