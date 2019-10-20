# Personal Blog
    
## Usage

Run locally with `bundle exec jekyll serve`

\_config.yml controls the site._ variables
* Header links can be manually controlled @ _config.yml -> header_pages

To add new header links, create a .md at / and make sure there's a proper set of headings
```
---
layout: page
title: About yihao
permalink: /about/
order: 10
---
```

To add a new post, create a new .markdown in _post
```
---
layout: post
title:  "Hola"
date:   2019-07-22 00:00:00 +0800
categories: overview
---
```

[User vs Project](https://jekyllrb.com/docs/github-pages/#project-page-url-structure)


## One-time setup

Steps
1. Install ruby ([Mac can be quite problematic](https://jekyllrb.com/docs/troubleshooting/#jekyll-amp-mac-os-x-1011))
2. `gem install bundler`
3. Add to Gemfile in ./ 
```
source 'https://rubygems.org'
gem 'github-pages', group: :jekyll_plugins
```
4. `bundle install`
5. Run locally with `bundle exec jekyll serve`

Might need to run `bundle update` from time to time. 

Bundler helps to manage dependencies for Ruby projects. Gemfile contains the dependencies that will be parsed and installed with `bundle install`

`open $(bundle show minima)`

## Notes

In-depth notes
* [Jekyll commands, including `jekyll serve`](https://jekyllrb.com/docs/usage/)
* [Structure](https://jekyllrb.com/docs/structure/)
* [Why do we need `bundle exec`](https://jdanger.com/what-does-bundle-exec-do.html)

Other links used
* https://help.github.com/en/articles/setting-up-your-github-pages-site-locally-with-jekyll
* https://karpathy.github.io/2014/07/01/switching-to-jekyll/

Other useful links
* [jekyllrb.com](https://jekyllrb.com/)
* [minima](https://github.com/jekyll/minima)
* [jekyll](https://github.com/jekyll/jekyll)

Useful but Unused
* https://github.com/github/personal-website

## Todo
* Google analytics
* Script to check for dead links
* Post preview on first page