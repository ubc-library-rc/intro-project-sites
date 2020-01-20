---
layout: page
title: Setup
permalink: /setup/
nav_order: 1
---

For this workshop, we'll build a site locally first, then publish it to the web when we're ready and have some content. In order to work locally, we have to make sure that our computer has all the necessary software installed. The steps to do this below require some familiarity with working in your command-line interface, so if you don't feel comfortable doing this, please refer another workshop in this series: [Intro to the Unix Shell](https://ubc-library-rc.github.io/intro-shell/).

## Windows OS


## Mac OS
The Mac operating system needs the Xcode suite to run several tools developers use to create software and applications. So to start, let's install it from the command line if you don't already have it.

### Install X-Code

First install **x-code**        
<code>$ xcode-select --install</code>    

This should install **gcc** and **git**, but let's make sure. Verify you are running gcc:    
<code>$ gcc --version</code>    
You should see a version number in your shell.    

Verify you have git:    
<code>$ git --version</code>     
Again, you should see a version number.    

### Install RVM   
Install the most recent stable version of **rvm**. Rvm will allow you to use different versions of Ruby (which we'll install next) for website projects, and for your operating system.    
<code>$ curl -L https://get.rvm.io | bash -s stable</code>

Now lets verify rvm was installed.    
<code>$ rvm --version</code>    

### Install Ruby with RVM    

Now install the most recent stable version of **Ruby** using rvm     
<code>$ rvm install "ruby-2.7.0"</code>    

Now then set that version as the default Ruby installation for our project    
<code>$ rvm --default use 2.7.0</code>    

Check that ruby is set to the version we configured    
<code>$ ruby -v</code>     

4. now generate the core Ruby documentation
  <code>$ rvm docs generate-ri</code>

5. navigate to a folder where you want to install your local site project (or another directory where you have projects like this):
  <code>$ cd documents/sites</code>

  and then create a new jekyll project called "[your name]-project-site":
    <code>$ jekyll new [your name]-project-site</code>

  Then cd into that new project:
    <code>$ cd [your name]-project-site</code>

6. install Bundler (we'll use this to install a new theme)
    <code>$ gem install bundler</code>

7. then finally cd into that directory and start the server to see the site:
    <code>$ cd [your name]-project-site</code>
    <code>$ jekyll serve</code>

  Go to 127.0.0.1:4000 and you should see your new blank site!
