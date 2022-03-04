---
layout: posts
title: Website guide
date: 18-02-2022
categories: Technology
---
# How I setup my website

Being unfamiliar with how to build a website myself, it proved slightly more difficult to make a free and somewhat stylish website from scratch, than I originally thought it would be. Here I describe the process I used to hopefully save someone else a bit of time. I use windows and don't know how this works for mac - sorry!

The criteria for my website was:
* Free
* Easy to manage and edit
* Flexible regarding content
* Include a blog

I found Jekyll combined with GitHub pages to meet these criteria. GitHub pages hosts a static site[insert link to static site] for free, and you get a  domain that is your GitHub username followed by .github.io. You are also able to use a custom domain. GitHub pages support markdown, which I find much easier to use than .html. I rely heavily on [this youtube guide](https://www.youtube.com/playlist?list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB) by Giraffe academy to setup this page.

## Building your website offline

### Installing the software

I found it useful to first build the site offline, and then put it online later, but you can also build it directly online.

Firstly, you need to download Ruby. To do this, go to rubyinstaller.org/downloads (link). Choose the latest version and download it. When prompted, check the run 'ridk install'. This opens a new window with three options. Install all three options. Press `1`, and then enter to install. Do the same for `2` and `3`. Don't run the MSYS2 64bit when prompted. To make sure you've installed ruby correctly, open the command prompt (just search for cmd in windows search.) Inside the commandprompt, we check if Ruby was installed correctly. To check this type `ruby -v`, to check if it's installed. Do the same for Gem: `gem -v`.

Now we can use Ruby to install Jekyll (the site generator.) Do to this type `gem install jekyll bundler` in the command prompt. This should install Jekyll.

### Building your website

Now we build our website using Jekyll. I built it on top of the minimal mistakes theme. First you download the minimal mistakes theme (use fork in GitHub, that is easiest). Now use your command line to move into your new website folder. It's nice to do this in a text editor. I use atom and download the platform-ide-terminal package to have a terminal in my editor. From this terminal you can serve up your website, so you can view it in your web browser as you start building it. To do this, type the command `bundle exec jekyll serve` in your terminal (make sure to be in the folder). If you get an error try to use the solution suggested [here](https://github.com/jekyll/jekyll/issues/8523) by first running the command `bundle add webrick` (I don't understand this error, but I got it when using another computer than my standard one.)

You're website is now being hosted locally on http://127.0.0.1:4000/. Type this into your web browser, and you can see you site. You will now see that you already have a basic site. You can explore this content in your text editor (or just opening the files in the explorer.)

## Customizing your site

The site at this point is very basic, and needs some customizing. In this post I describe the most important things for the minimal mistakes theme, but how you customize differs from theme to theme. Add your information in the _config.yml file. This information will be used across the site.

Things to do with the minimal mistakes theme:

* Add a _pages folder, for your sites
* Remove stuff from the footer.
* The index file should be the html site in the minimal mistakes theme. For some reason a faulty html file is created by default for me. Probably a me-issue, but I just use html for this one page.


**To sum up the process**: Install Ruby > Install Jekyll > Use Jekyll to make site >  

## Getting your website online

Upload your offline website as a GitHub repository

Setting up the repository as a GitHub page.

Now you should be able to see your website on the domain provided to GitHub. The first page is the index file in the website. If you want your own domain, you can enter it under the GitHub Pages settings. You can buy a domain from where-ever you want.

### Sitemap

You need to provide something called a sitemap, if you want people to be able to find your website. I still don't fully understand how this works, but here's what I did to make my website google-able.

## Other options

### Wordpress

### Squarespace

### Wix
