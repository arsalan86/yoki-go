# yoki-go (よき-go)

![Deploys by Netlify](https://www.netlify.com/img/global/badges/netlify-light.svg "Deploys by Netlify")

A clean, minimal, netlify ready theme for Hugo, derived from [hucore](https://github.com/mgjohansen/hucore).

This is a work in progress. I've uploaded it in order to be able to deploy to Netlify for live testing. Netlify integration is one of my main goals for this theme. The master branch (currently locked to #0ed1718) is deployed [here](https://yoki-go.netlify.com/).

Visually, the theme is nearly identical to [hucore](https://github.com/mgjohansen/hucore) with a few layout and font changes. I've derived from hucore (as opposed to forking it) because it is a nice clean theme that serves my purpose well: I wanted a starting point for my experimentations with Hugo and continious deployments on Netlify. This theme is a small part of a larger project I'm working on that incorporates Hugo and the Netlify API. There are no plans for any significant deviations from hucore/Hemingway in terms of style. 

## Installation

Navigate to the root of your Hugo site and add yoki-go as a submodule into the themes folder:

```
$ git submodule add https://github.com/arsalan86/yoki-go themes/yoki-go
```

The exampleSite folder contains example content used in the live preview, as well as the `config.toml` file. Copy the `config.toml` file to the root of your hugo site, overwriting the existing one if necessary. You may copy the example content from the content folder if you wish.

## Configuration

Configuration is straightforward. Edit the `config.toml` file to suit your requirements.

The `blogroot` setting points to the folder where your blog posts are. A paginated list of all posts in this folder will be shown on the homepage, underneath all content in the `_index.md` page. If you do not wish to display any posts on the homepage, simply comment the line, or delete it.

If you wish to add top level pages to your site (work/about/contact etc), place them in the root folder, and add the following to their front matter:

```
type: "singlepage"
layout: default
```

Hugo will then use the template in `layouts\singlepage\default.html` to process these pages. You can change the values for `type` and `layout`. Hugo looks for a template in `layouts\<type>\<layout>.html`.

## Todo:

- Performance tweaks: remove above the fold scripts

## Roadmap:

- Netlify integration via a python script: this should be as simple as invoking the script, inputting your credentials, git repo and deploying
- Template variables in css, css optimization and simplification to allow easier customization