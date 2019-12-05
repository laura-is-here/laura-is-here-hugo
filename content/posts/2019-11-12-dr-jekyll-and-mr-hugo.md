---
title: Dr. Jekyll and Mr. ... Hugo?
author: Laura
date: 2019-11-12
draft: true

---
## My experiences with two mainstays in the world of static sites

As a primarily self-taught designer and developer, discovering static site generators marked a breakthrough in my web development skills and, more importantly, work flow and build process.

<!--more-->

I cut my teeth on html and css in plain text files uploaded straight to the server. The first iteration of this site was actually hosted on {{< anchor "neocities" "https://neocities.org" >}} and was, in fact, primarily edited in their in-browser editor!

It wasn't until the folks with {{< anchor "Long Beach Anarchist Collective" "https://anarchistlb.org" >}} requested an events page that I started delving more into content management systems and, {{< anchor "after ruling out Wordpress as bulky and unnecessary" "https://gettingthingstech.com/hugo-vs.-wordpress-page-load-speed-comparison-hugo-leaves-wordpress-in-its-dust/" >}}, discovered {{< anchor "Jekyll" "https://jekyllrb.com" >}}.

## Jekyll

Jekyll was initially appealing to me due to its home in the realm of {{< anchor "Ruby" "https://ruby-lang.org/" >}}, a language and environment with which I was already somewhat familiar.

Jekyll presented several immediate advantages to my work flow and build process:

* live rendering of the site on a local server
* the ability to use "includes" to easily recycle components like menus, headers, etc.
* integration with Sass/SCSS

I transitioned an early version of this site, as well as {{< anchor "Tiffany Hooton's site" "tiffanyhootontherapy.neocities.org" >}}, to use Jekyll before starting a more full-flegded blog for {{< anchor "Long Beach Anarchist Collective" "anarchistlb.org" >}}. The results, both in terms of development workflow and the final product, were huge improvements to the barebones HTML and CSS that I had worked with before.

### Cons of Jekyll

Jekyll was not without some cons. As I started delving into the world of NPM and Node more, I found that managing Node modules alongside Ruby was a tad tedious for someone of my skill level, and getting things as simple as Autoprefixer and PostCSS set up within Ruby and Jekyll was less than intuitive and frustrating due to lack of good documentation and unmaintained packages.

As a workaround I began using MAKE to set up the development environment and get the best out of NPM and Ruby based tools.

However, as this development environment got more complex, I began running into problems with build speeds. Jekyll slowed down just a little bit, taking anywhere between 5 - 7 seconds to regenerate the live preview in the browser. While not a _long_ time, the extended periods waiting to click refresh in the browser after every save add up and, again, introduce more frustration to developing.

## Hugo: something faster