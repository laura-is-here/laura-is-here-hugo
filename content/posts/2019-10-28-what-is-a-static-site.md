---
title: What is a static site?
author: Laura
date: "2019-10-28"
---
At one point in the now vast history of the web, essentially all websites were **static**&mdash;mostly meaning that they were not **dynamic**.

To understand this and the implications for us now, let's take a look at some of the work that goes on behind the scenes when a user visits a site.

<!--more-->

## Servers, browsers, domains&mdash;oh my!

- A **site** is a collection of **pages**, usually with a consistent style, grouped together for a particular purpose

Let's say we've made a site for our pet frog, named timothy. we might have a landing page that introduces timothy, which itself contains navigation links to other pages on the site, such as a page for timothy's favorite foods, timothy's hobbies, etc.

- The **pages** of a site are text files written in markup languages like html that browsers can interpret and present nicely

Before your browser can get to the pages, however, it has to know where to get them. This is where **domain names** come in. You register the domain at {{< anchor "myfrogtimothy.me" "http://myfrogtimothy.me" >}} with a domain registrar so that when someone types in {{< anchor "myfrogtimothy.me" "http://myfrogtimothy.me" >}} into their browser, this **domain name server** knows where to get the **pages** for your **site**. 

- For our purposes, we want traffic directed to our landing page for timothy, which we store on a server that is able to respond to a browser's request for our files. This server is positioned to understand what the browser is requesting from it

With static sites, this process is that simple. You type the name of a site into your browser, a domain name server points your browser to the web server where the files for that site are being served, and that server send your browser the requested file for your viewing pleasure.

## The problem

As sites started getting larger and receiving more traffic, this model of serving static files became harder to manage.

**Enter, dynamic sites.**

Dynamic sites do more work on what's referred to as *the backend*&mdash;all the stuff that goes on behind the scenes.

When your browser requests a page from a dynamic site, the server responds by first putting together pieces, usually from a **database**, and *creates* the **page** you asked for then and there.

Dynamic websites have been an important step in the path to the web we all know and love today, allowing a site's content to remain flexible and saving developers from a lot of copying and pasting while managing sites with sometimes thousands of **pages**.

Managing websites using a database *makes sense*, especially when many of the same pieces of information are being repeated over and over between different pages.

Dynamic sites addressed *a problem* that web developers, clients, and users needed an answer to.

So, now that we've come all this way, why static sites again?

## The new problem(s)

If you've ever set up a Wordpress site, you've set up a dynamic site. congratulations! You've used databases and a content management system (cms) to manage and serve up your content.

If you've ever forgotten to update your Wordpress site, or tried to make fine-tuned customizations to the theme or migrate your content to another service, or faced slow loading times, or...well, you get the point: dynamic sites consist of so many moving parts that they require *maintenance* to remain up and running. And often that's skilled maintenance that is time-consuming and costly.

## Static sites to the rescue

Modern static sites built with static site generators and other build tools take a different strategy on addressing the problems that dynamic sites were designed to tackle in the first place.

Need a database to integrate and manage the content of your site?

Static sites have you covered with easy to use, plain text database files that generate content for your site at the time it's built (before or during its upload to your server)

Running a personal blog to boost your seo?

Static sites have you covered with custom cms integration and easy blogging management.

Worried about security, maintainence, and all the technical issues that lurk around the corner with your site?

Static sites have you covered by minimizing the number of components that must be maintained and kept up to date.

## The bottom line

Dynamic sites make sense for a large majority of developers, clients, and users. If there is enough moving content involved in your site and the resources are there to maintain it and keep developers, clients, and users happy, then, by all means, go dynamic!

But if you're an individual or organization with an old Wordpress site (the kind that has cobwebs piling up on the admin dashboard) that you use to make your presence known online, consider whether or not you actually require the type of service that dynamic sites provide.