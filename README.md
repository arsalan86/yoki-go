# yoki-go (よき-go)
![Deploys by Netlify](https://www.netlify.com/img/global/badges/netlify-light.svg "Deploys by Netlify")

A clean, minimal, netlify ready theme for Hugo, derived from [hucore](https://github.com/mgjohansen/hucore).

This is currently a work in progress. I've uploaded it in order to be able to deploy to Netlify for live testing. Netlify integration is one of my main goals for this theme. The master branch (currently locked to #0ed1718) is deployed [here](https://yoki-go.netlify.com/)

## Installation

Navigate to the root of your hugo site and clone yoki-go into the themes folder:

```
$ git submodule add https://github.com/arsalan86/yoki-go themes/yoki-go
```

The exampleSite folder contains example content used in the live preview, as well as the `config.toml` file. Copy the `config.toml` file to the root of your hugo site, overwriting the existing one if necessary. You may copy the example content from the content folder if you wish.

## Todo:

- Organize theme structure
- Add filler content for preview
- Include script for netlify deployment
- Performance tweaks: remove above the fold scripts