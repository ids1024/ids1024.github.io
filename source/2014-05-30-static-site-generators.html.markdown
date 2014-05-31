---
title: Static Site Generators
date: 2014-05-30 20:09 PDT
tags:
---

There are essentially two ways to create a website. The most popular method is to use a CMS such as Drupal, Joomla, Wordpress, etc. This method allows for web-based WYSIWIG editors for site content, extensions, user login, comments, and various other features. It is also slower and less secure. Each time a page is loaded, the server must generate the page, often with a php script. There are methods to improve this, but nothing will be more efficient than plain, old fashioned, static html.

Static html is also more secure. A CMS allows for login to make changes to site content. Static html has no login, and indeed no code running on the server. The server may still have security flaws, but the static html is not at fault.

But static html has its own problems. Perhaps you wish to update the copyright date in your site's footer. You must change every page. If your website has five pages, this is not a problem. If it has five hundred, it might take a while, though this is a relatively trivial change. This could be remedied by php or server side includes, but this would result in the aforementioned performance issues, and possibly even insecurity.

What if you could take the best features of both a CMS and static html? Perhaps you could use a form of CMS, but have it generate static html instead of rendering the page on each load. Such a thing exists, and it is called a static site generator.

There are countless static site generators. I use [Middleman](http://middlemanapp.com), but there may be better ones, since I have not tried many. Middleman, like many static site generators, is implemented in Ruby. Static site generators implemented in Ruby can utilize tools designed for Ruby on Rails.

There are many legitimate reasons to use a CMS, but I prefer Middleman. It also fits better into a command line workflow. And thus, I am using Middleman for this site.
