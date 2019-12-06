---
title: Dr. Jekyll and Mr. ... Hugo?
author: Laura
date: 2019-11-12
draft: true

---
## My experiences with two mainstays in the world of static sites

As a primarily self-taught designer and developer, discovering static site generators marked a breakthrough in my web development skills and, more importantly, work flow and build process.

<!--more-->

I cut my teeth on HTML and CSS in plain text files uploaded straight to the server. The first iteration of this site was actually hosted on {{< anchor "neocities" "https://neocities.org" >}} and was, in fact, primarily edited in their in-browser editor!

It wasn't until the folks with {{< anchor "Long Beach Anarchist Collective" "https://anarchistlb.org" >}} requested an events page that I started delving more into new solutions for building out new pages quickly and, {{< anchor "after ruling out Wordpress as bulky and unnecessary" "https://gettingthingstech.com/hugo-vs.-wordpress-page-load-speed-comparison-hugo-leaves-wordpress-in-its-dust/" >}}, discovered {{< anchor "Jekyll" "https://jekyllrb.com" >}}.

## Jekyll

Jekyll was initially appealing to me due to its home in the realm of Ruby, a language and environment with which I was already somewhat familiar, as well as its flexibility and accessibility for new users.

Jekyll presented several immediate advantages to my work flow and build process:

* live rendering of the site on a local server
* the ability to use "includes" to easily recycle components like menus, headers, etc.
* integration with Sass/SCSS

I transitioned an early version of this site, as well as {{< anchor "Tiffany Hooton's site" "tiffanyhootontherapy.neocities.org" >}}, to use Jekyll before starting a more full-flegded blog for {{< anchor "Long Beach Anarchist Collective" "https://anarchistlb.org" >}}. The results, both in terms of development workflow and the final product, were huge improvements to the barebones HTML and CSS that I had worked with before.

### Cons of Jekyll

Jekyll was not without some cons. As I started delving into the world of NPM and Node more, I found that managing Node modules alongside Ruby was a tad tedious for someone of my skill level, and getting things as simple as Autoprefixer and PostCSS set up within Ruby and Jekyll was less than intuitive and frustrating due to lack of good documentation and unmaintained packages.

As a workaround {{< anchor "I began using GNU Make" "https://simpleit.rocks/ruby/jekyll/tutorials/how-to-add-bootstrap-4-to-jekyll-the-right-way/" >}} to set up the development environment and get the best out of NPM and Ruby based tools.

However, as this development environment got more complex, I began running into problems with build speeds. Jekyll slowed down just a little bit, taking anywhere between 5 - 7 seconds to regenerate the live preview in the browser. While not a _long_ time, the extended periods waiting to click refresh in the browser after every save add up and, again, introduce more frustration to developing.

## Hugo: something faster

Where Jekyll is flexible and approachable, my first impressions of Hugo were the opposite.

Written in Go, {{< anchor "Hugo, _the world's fastest framework for building websites,_" "https://gohugo.io" >}} has a much higher learning curve. But there are also some immediate advantages:

* installed as a pre-compiled binary (no dealing with NPM, Ruby, etc.)
* built-in asset pipeline for PostCSS, CSS minification, and image optimization
* live rendering and generation that is _blazing_ fast

With the {{< anchor "quick start guide" " https://gohugo.io/getting-started/quick-start/" >}} supplied in the documentation, you will absolutely have Hugo up and running in no time—if you're okay with using a pre-built theme.

I am _not_ a theme type of person. Web design and frontend development are attractive to me because I'm a picky and detailed tinkerer, so any theme I'm using has to be wide open for modifications.

With some knowledge, Hugo's themes are absolutely open to customization, but that's not something a beginner will be ready to dive into, and since themes are independently maintained, you're often working with documentation that is not fully fleshed out or out of date, especially since Hugo is much more rigid when it comes to templating and directory structures.

All that being said, if you spend some time with Hugo and take your time with the documentation, Hugo is really worth it. It's incredibly fast and includes plenty of built-in functionality that will be useful if working with NPM and Node is not your cup of tea.

Once you're familiar with some of the quirks of the setup, Hugo will be a very powerful tool in your arsenal.

## The bottom line

I've begun moving many of my Jekyll projects over to Hugo. Jekyll is a fantastic tool, but Hugo suits my needs a bit better and cuts down on a lot of time spent with configuration and managing assets that Jekyll can require.

If you're new to static site generators, I can't recommend {{< anchor "Jekyll's step by step tutorial" "https://jekyllrb.com/docs/step-by-step/01-setup/" >}} enough to get you up and running and tinkering away. Hugo, on the other hand, takes some more getting used to in order to really get a firm grasp on how to fully utilize it, but it is very powerful, very fast, and very worth it. {{< anchor "Did I mention it's fast?" "https://forestry.io/blog/hugo-vs-jekyll-benchmark/" >}}