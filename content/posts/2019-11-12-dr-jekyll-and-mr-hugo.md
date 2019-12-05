---
title: Dr. Jekyll and Mr. ... Hugo?
author: laura
date: 2019-11-12
draft: true

---
## my experiences with two mainstays in the world of static sites

as a primarily self-taught designer and developer, discovering static site generators marked a breakthrough in my web development skills and, more importantly, work flow and build process.

<!--more-->

i cut my teeth on html and css in plain text files uploaded straight to the server. the first iteration of this site was actually hosted on {{< anchor "neocities" "https://neocities.org" >}} and was, in fact, primarily edited in their in-browser editor!

it wasn't until the folks with {{< anchor "Long Beach Anarchist Collective" "https://anarchistlb.org" >}} requested an events page that i started delving more into content management systems and, {{< anchor "after ruling out wordpress as bulky and unnecessary" "https://gettingthingstech.com/hugo-vs.-wordpress-page-load-speed-comparison-hugo-leaves-wordpress-in-its-dust/" >}}, discovered {{< anchor "Jekyll" "https://jekyllrb.com" >}}.

## Jekyll

jekyll was initially appealing to me due to its home in the realm of {{< anchor "ruby" "https://ruby-lang.org/" >}}, a language and environment with which i was already somewhat familiar.

jekyll presented several immediate advantages to my work flow and build process:

* live rendering of the site on a local server
* the ability to use "includes" to easily recycle components like menus, headers, etc.
* integration with sass/SCSS

i transitioned an early version of this site, as well as tiffanyhootontherapy.neocities.org, to use Jekyll before starting a more full-flegded blog for anarchistlb.org. the results, both in terms of development workflow and the final product, were huge improvements to the truly barebones HTML and CSS that I had worked with before.

### cons of Jekyll

Jekyll was not without some cons. as i started delving into the world of npm and node more, I found that managing node modules alongside ruby was a tad tedious for someone of my skill level, and getting things as sime as autoprefixer and postcss set up within ruby and Jekyll was less than intuitive and frustrating due to lack of good documentation and unmaintained packages.

as a workaround I began using make to set up the development environment and get the best out of npm and ruby based tools.

however, as this development environment got more complex, I began running into problems with build speeds. Jekyll slowed down just a little bit, taking anywhere between 5 - 7 seconds to regenerate the live preview in the browser. while not a _long_ time, the extended periods waiting to click refresh in the browser after every save add up and, again, introduce more frustration to developing.

## hugo: something faster