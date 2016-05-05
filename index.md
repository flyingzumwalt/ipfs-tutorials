---
layout: default
title: Home
---

## Create a Curriculum with Git, Jekyll and Github Pages

Use this template to create a web-based curriculum that can be hosted on Github Pages or any jekyll server.

There's no database-just markdown files and a couple HTML templates. That's all. Everything is in a github repository, so people can fork the curriculum, add Courses, Modules and Activities, and then submit pull requests or host their own copies of the Curriculum.

## Usage

Download the contents of the git repository
Add your own content into the "curriculum" directory

### Hosting your curriculum on Github Pages

It's easy to host your curriculum on Github pages. Github's help pages about [Using Jekyll as a static site generator with GitHub Pages](https://help.github.com/articles/using-jekyll-as-a-static-site-generator-with-github-pages/) should provide the info you need to get going.

### Applying Styles and templates

There are lots of Jekyll Themes out there that you can apply to your curriculum.  This template is set up to work with the [pool/hyde](https://github.com/poole/hyde) theme, but using it with another theme is relatively easy.

If you already have your curriculum in a git repository, you can apply your content on top of a template like this (assuming your curriculum content is in the master branch). _Note: you will probably have to resolve some merge conflicts when you run `git merge master`_
```
git remote add hyde git@github.com:poole/hyde.git
git fetch hyde
git checkout -b gh-pages hyde/master
git merge master  
git commit -m"apply curriculum content on top of hyde"
```

### Serve your Curriculum anywhere with Jekyll

In the root of your curriculum content, run

```
bundle install
bundle exec jekyll serve
```

See the [Setting up your GitHub Pages site locally with Jekyll](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/) for more info and troubleshooting.
