---
published: true
layout: post
title: Hello World
quote: How I started this Jekyll blog.
image: 
  url: ""
  source: null
color: #589FF1  
posted: Published 
video: false
comments: true
---

## Hello World!

No, this is not a typical default hello world post on some Wordpress blog.

I have successfully installed [Jekyll](http://jekyllrb.com)! And deployed it on [Github Pages](https://pages.github.com). I came across [Karan's blog](http://karan.github.io) and he told me the site is using Jekyll. I have been struggling to decide whether I should have my blog on Wordpress/Jekyll/Medium/[Svbtle](https://svbtle.com)(I will write about on a new post some other time), but what really pushed me to start this Jekyll blog is because I stumbled across [this beautiful theme I could use](http://jekyllthemes.org/themes/thinny) from [Jekyll Themes](http://jekyllthemes.org/).

{% include image.html url="/media/2014-04-23-hello-world/thinny.png" width="100%" description="Screenshot of Thinny theme on Jekyll Themes." %}

I have problem installing Xcode Command Line Tools on my computer since [CodeAcrossSeattle Hackathon](https://medium.com/p/1a741836f226). Thank god I finally [found the solution on Stack Overflow](http://stackoverflow.com/questions/4518031/issue-installing-ruby-by-rvm-error-while-running-configure), I was installing the Command Line Tools on the wrong directory previously:

~~~
after which make sure Xcode command line tools is pointed correctly using this command

xcode-select -p

Which might show some path like

/Applications/Xcode.app/Contents/Developer

Change the path to correct path using the switch command

xcode-select --switch /Library/Developer/CommandLineTools/
~~~

Also an important reminder that we need to run this command in the terminal everytime we try to run RVM:

~~~
source /Users/chipdonglim/.rvm/scripts/rvm
~~~

{% include image.html url="/media/2014-04-23-hello-world/terminal.png" width="100%" description="Ruby is successfully installed after I changed the Xcode directory." %}

### I would like to thank these post authors for writing these resources, they helped me a lot:
- [Get Started With GitHub Pages (Plus Bonus Jekyll)](http://24ways.org/2013/get-started-with-github-pages/)
- [Installing Ruby & Jekyll on Mac OS X](http://andytaylor.me/2012/11/03/installing-ruby-and-jekyll/)

Though I would like to point out some errors on Andy Taylor's blog post, they were probably outdated:

The correct command for installing Homebrew:<br>
`ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"`<br>
If this is not working you can always refer to the updated command on [Homebrew's page](http://brew.sh/).

The correct command for starting Jekyll server:<br>
`jekyll serve` not `jekyll --server`

I also came across [Prose.io](http://prose.io), a content Editor for Github which allows users to preview the changes directly on Markdown, and it could function similar to Wordpress editor, which I am used to for writing blog posts. You can read more about Prose.io [here](developmentseed.org/blog/2012/june/25/prose-a-content-editor-for-github/).

{% include image.html url="/media/2014-04-23-hello-world/prose.png" width="100%" description="Interface for Prose.io" %}

## Setting up Subdomain
Github has [execellent documentation on setting up subdomain](https://help.github.com/articles/setting-up-a-custom-domain-with-github-pages). An important step is to setup the A records that resolve to the following IP addresses:

~~~
192.30.252.153
192.30.252.154
~~~

GoDaddy takes a while to forward, so it's really helpful for me to keep track of whether the domain name has been forwarded using this command:

`dig example.com +nostats +nocomments +nocmd`

## Some other beautiful Jekyll themes:
- [Hikari](http://jekyllthemes.org/themes/hikari/)
- [Incorporated](http://jekyllthemes.org/themes/incorporated/)

## Credits
[Thinny Theme](http://jekyllthemes.org/themes/thinny/) built by [Camporez](http://camporez.com)<br>
Proudly built on [Jekyll](http://jekyllrb.com/)<br>
Hosted on [Github Pages](https://pages.github.com/)
