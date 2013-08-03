#Tech Hamlet

This is the source code for [TechHamlet.com](http://techhamlet.com). It is built on [Octopress](http://octopress.org/). I have done a lot of customization to the design and the basic layout. Here are some features that I have managed to add (there are more) :

####Features added :

* Featured images for posts. Every post will have a `fimage` tag. The site will pull the image path from this tag and use it to display a post image in the index and in the sidebar recent posts.
* Featured posts. If the `featured` tag is set to true in a post, the blog index will style that post differently. (For example, add a bigger image to it)
* Auto excerpts. Octopress have excerpts. The only thing is you have to add the `<!--more-->` tag manually. I imported nearly 1,500 posts from my old wordpress setup. I can't go through all these posts and add the more tag manually! So, I used the `truncatewords` method in Liquid Templates like this :

{{ post.content | strip_html | truncatewords: 30 }}

* One of the best things about Octopress is that you can get free hosting on Github. But there's a problem... If you upload the source to Github (Free account), anyone can get your posts easily (Thats what I think. Im not sure). You can push the source to a different place like Bitbucket. But it won't make the source open. So, I pushed the posts, pages and their images to my private repository in Bitbucket and left the source in Github. This bring another problem. You need to push the source, pages, posts and images separately to their own origins which can become a big headache. But, I created two scripts to **commit** and **push**. To take care of all the repositories from one script. I will write about it in [Tech Hamlet](http://techhamlet.com/) in the near future. (They are not included in the source).
* And there are some more tiny things I added...

####Major problems :

* The current major problem I'm facing is the long archive pages! Octopress doesn't paginate category and archive pages. In my blog archive, I have nearly 1,500 posts! If any one know how to fix it, [please let me know](http://techhamlet.com/contact/)


###License

<span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">**Tech Hamlet Site Design**</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://techhamlet.com/" property="cc:attributionName" rel="cc:attributionURL">Tech Hamlet</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/deed.en_US">Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License</a>. <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/deed.en_US"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/3.0/80x15.png" /></a><br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="http://octopress.org/" rel="dct:source">http://octopress.org/</a>.<br />Permissions beyond the scope of this license may be available at <a xmlns:cc="http://creativecommons.org/ns#" href="http://techhamlet.com/contact/" rel="cc:morePermissions">http://techhamlet.com/contact/</a>.

You can edit and share the design (with the layout) or even use it on your own site. But you have to link back to [Tech Hamlet](http://techhamlet.com/) and give some credit to us.

**Tech Hamlet Site Content (All post and page content (the original mark down versions))** are copy protected! **Copyright © 2009 - 2013 Tech Hamlet - Sri Lanka (All rights reserved)**. (Don't worry, they are not uploaded to Github. Everything in this Github repository is open and use the above mentioned Creative Commons license!) You are not allowed to copy any posts from our site. If you do so, Google will immediately add penalties for you (for posting duplicate content) and your web site will go down! So, be-careful!

___

## What is Octopress?

Octopress is [Jekyll](https://github.com/mojombo/jekyll) blogging at its finest.

1. **Octopress sports a clean responsive theme** written in semantic HTML5, focused on readability and friendliness toward mobile devices.
2. **Code blogging is easy and beautiful.** Embed code (with [Solarized](http://ethanschoonover.com/solarized) styling) in your posts from gists, jsFiddle or from your filesystem.
3. **Third party integration is simple** with built-in support for Pinboard, Delicious, GitHub Repositories, Disqus Comments and Google Analytics.
4. **It's easy to use.** A collection of rake tasks simplifies development and makes deploying a cinch.
5. **Ships with great plug-ins** some original and others from the Jekyll community &mdash; tested and improved.


## Documentation

Check out [Octopress.org](http://octopress.org/docs) for guides and documentation.


## Contributing

[![Build Status](https://travis-ci.org/imathis/octopress.png?branch=master)](https://travis-ci.org/imathis/octopress)

We love to see people contributing to Octopress, whether it's a bug report, feature suggestion or a pull request. At the moment, we try to keep the core slick and lean, focusing on basic blogging needs, so some of your suggestions might not find their way into Octopress. For those ideas, we started a [list of 3rd party plug-ins](https://github.com/imathis/octopress/wiki/3rd-party-plugins), where you can link your own Octopress plug-in repositories. For the future, we're thinking about ways to easier add them them into our main releases.


## License
(The MIT License)

Copyright © 2009-2013 Brandon Mathis

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the ‘Software’), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED ‘AS IS’, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


#### If you want to be awesome.
- Proudly display the 'Powered by Octopress' credit in the footer.
- Add your site to the Wiki so we can watch the community grow.