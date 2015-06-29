# Make Technology Website

Welcome to the thrilling world of Make Technology, where great things happen.

## Environment Setup

In order to modify, improve, or add new features to the Make Technology website you must clone its repository from Github. This is also required whether you want to write a blog post. This can be done using the git CLII with the following command:

	git clone git@github.com:ssampaoli/ssampaoli.github.io.git

## How to write a blog

First, you have to install Jekyll, a simple, blog-aware static site generator. To install it (and to know more about it) please follow the following [Github guide](https://help.github.com/articles/using-jekyll-with-pages/#installing-jekyll).

After installing Jekyll you can start writing your blog post following these simple steps:

 - Write your blog post with your favorite text editor using Markdown syntax. Save it with the .md extension.
 - If you want to use images place them in /img/some_path and referenced them from your blog post.
 - If it is the first time you write a blog you should:
 	- Add your author information to the authors.yml file of the _data folder.
 	- Add your avatar photo to the /img folder. This photo must be referenced from the authors.yml file.
 - When writing your post make sure that the front matter has at least the the following content:
```txt
---
layout: post
title: The title of the post
category: blog
excerpt: "A brief description of the blog post."
modified: 2015-06-24
tags: [tag1, tag2, tag3, ...]
comments: true or false
author: the id of the author as appear in the authors.yml file
---
The content of the post is written here in Markdown syntax.
```
 - You may also add a feature image, an image that will appear at the top of your post, adding the front matter attribute `image: feature:` (Please see the sample-post.md file for this option).
 - You should write and save your blog posts in the _drafts folder before publishing. This way you can test and verify that the content and layout of your post is the one you desire. Besides, this is a great way to allow others team members review your posts before publishing. To preview your site with drafts, simply run `bundle exec jekyll serve --drafts`.
 - Once you (or the people you want) has verified that the post is correct you can publish it moving the post file from the _drafts folder to the _posts/blog/ folder. If you haven't done it before, remember to name it in the format year-month-day-title.md, and include the front matter at the top of the post.
 - Commit the post’s Markdown file, and push to our GitHub repository.
 - That’s it! Just wait for GitHub Pages to rebuild your website. This typically takes under 10 seconds.

Too many words...it is often better to have and example and copy the structure and some content from it. Then you can take a look at the sample post placed in the _drafts folder to see how Jekyll works. Its file name is sample-post.md. Remember that you can have it working by running the command `bundle exec jekyll serve --drafts` in the command line.

===

For more Jekyll details, read [documentation](http://jekyllrb.com/).
