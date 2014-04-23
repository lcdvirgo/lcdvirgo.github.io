---
published: true
layout: post
title: Hello World
quote: How I started this Jekyll blog.
image: 
  url: "/media/2014-02-27-hello-cosette/cover.jpg"
  source: null
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

#### Some other beautiful Jekyll themes:
- [Hikari](http://jekyllthemes.org/themes/hikari/)
- [Incorporated](http://jekyllthemes.org/themes/incorporated/)
