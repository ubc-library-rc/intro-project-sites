---
layout: default
title: What is Jekyll?
permalink: /jekyll/
parent: Summary
nav_order: 2
---
### Jekyll
Jekyll is a popular site generator that transforms plain text documents (Markdown, HMTL, CSS, etc.) into static sites that can easily be used for blogs and informational websites. Jekyll works very well with traditional Git and GitHub workflows, and so if you are already familiar with those, Jekyll site building will seem straightforward. If you aren't, don't worry – this workshop is meant for beginners. Jekyll is written in Ruby and so you'll notice some Ruby-specific terminology (like "Gems").

### Anatomy of your Jekyll site
Let's take a look at your new Jekyll installation and see what's there. Most of the information here is from the [Official Jekyll documentation](https://jekyllrb.com/docs/){:target="_blank"}.
#### File Structure
The default Jekyll package will install a directory of files that make up your site. Canonical information about this [file structure](https://jekyllrb.com/docs/structure/){:target="_blank"} can be found here. Your new installation should have installed a directory with a file structure that looks similar to this:
```
.
├── _config.yml
├── _drafts
├── _includes
|   ├── footer.html
|   └── header.html
├── _layouts
|   ├── default.html
|   └── post.html
├── _posts
|   ├── 2020-02-10-welcome-to-jekyll.md
├── _sass
|   ├── _base.scss
|   └── _layout.scss
├── _site
├── .jekyll-metadata
├── 404.html
├── about.md
├── Gemfile
└── index.html
```
Many of the files listed here are used by Jekyll to "transform" your content into a site – which is generated on-the-fly, and stored in the folder **_site**. For this workshop we're going to concentrate on the essentials, including the **config.yml** file, posts, pages, and styling.
#### Posts

#### Front Matter

#### Pages

## Start your Jekyll server
Jekyll uses a web server to transform its content into a website. So in order to see your live site, we'll need to start a local web server to see our development sites live in your browser.    

In your Unix shell start your server using the command:    
<code>$ jekyll serve</code>     

Now head to [http://127.0.0.1:4000/](http://127.0.0.1:4000/){:target="_blank"} to see your site in your browser. You should see the default Jekyll site homepage and styling:    


![Blank Site](/img/blanksite1.png){: width="600px" border="1px, red"}  


You may really like the way this default site looks and can use it as-is. Or, you might want to start building your own site from scratch. Each direction comes with its own costs and benefits. For this workshop, we're going to customize the default site and add some content. Then we'll show you how you can install themes that fit your project's look, feel, and desired functionality.    

### Customize your _config.yaml
Notice that your site's title and email are still set to the generic default. "Your awesome title", "your-email@example.com", and other settings can be re-configured in the <code>config.yml</code> file.
