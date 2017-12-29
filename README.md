# LIM -A Theme For HEXO-
LIM, it is an abbreviations of “_Less is more_”. A sophisticated morden flat design completed this clean, easy, wonderful theme.

## **BEFORE USING**
>LIM IS NOW STILL ALFA VERSIOM。

> PLEASE REQUEST THE PROBLEM TO US TO MAKE THE THEME BETER😉

***

 ### STATE OF FRONT-END DEVELOP
 - "[✓]" Means Finished "[ ]" Means Haven't Finished.   

- [x] Footer Social-link icon quote from Font-Awesome
- [x] Search Box Effect
- [x] Import Pace.js For Loading Effect
- [x] Build New "About Page"
- [ ] Index.ejs & layout.ejs Rebuild
- [ ] Picture Display Effect Rebuild
- [x] Change Markdown Render Engine
- [x] Support Checkbox With MD

### STATE OF BACK-END DEVELOP
 - "[✓]" Means Finished "[ ]" Means Haven't Finished.

- [x] Optimise Footer.ejs & config.yml Efficiency
- [x] ~~Local Comments System Build~~ Support Disqus
- [ ] Local Search System Build
- [ ] Optimice CSS & JS Animation Performance    

  ***   

### Usage
1. cd To Your `Root` Directory Of HEXO   

   `$ cd ~/Your-Root-Derectory-Of-Hexo/`

2. Clone Files And Install Necessery Parts    

   `$ clone https://https://github.com/CarterJimmy/LIM.git themes/LIM`   
   `$ npm install hexo-renderer-sass --save`  
   `$ npm install hexo-tag-fontawesome --save`    
   `$ npm install hexo-generator-tag --save`    
   `$ npm install hexo-generator-feed --save`    
   `$ npm install hexo-tag-aplayer --save`

3. Change the `themes` property in `_config.yml`     

   `theme: LIM`

4. Customize And Apply    
Run `hexo server` to test the theme at local.    
Run `hexo deploy -g` to apply new theme for your Page

***

### Other
To use the checkbox function, you have to remove the default markdown-render-engine and install `hexo-renderer-markdown-it` for new one.   
Here is the step for install.

1. Move to your `root` Directory Of HEXO

  `$ cd ~/Your-Root-Derectory-Of-Hexo/`

2. Remove the default renderer, and install new renderer.

  `$ npm uninstall hexo-renderer-marked --save`   
  `$ npm install hexo-renderer-markdown-it --save`

3. For using the checkbox function, you have to install `markdown-it-checkbox` plugin.

  `$ cd node_modules/hexo-renderer-markdown-it/`    
  `$ npm install markdown-it-checkbox --save`

4. Change your root `_config.yml`

 ```yaml
 # Markdown-it config
## Docs: https://github.com/celsomiranda/hexo-renderer-markdown-it/wiki
markdown:
  render:
    html: true # Doesn't escape HTML content so the tags will appear as html.
    xhtmlOut: false # Parser will not produce XHTML compliant code.
    breaks: true # Parser produces `<br>` tags every time there is a line break in the source document.
    linkify: false # Returns text links as text.
    typographer: true # Substitution of common typographical elements will take place.
    quotes: '“”‘’' # "double" will be turned into “single”
                   # 'single' will be turned into ‘single’
  plugins:
    - markdown-it-abbr
    - markdown-it-checkbox # Enable the checkbox function
    - markdown-it-emoji # If you're looking for the Emoji function, you have to install this plugin
    - markdown-it-footnote
    - markdown-it-ins
    - markdown-it-sub
    - markdown-it-sup
  anchors:
    level: 2 # Minimum level for ID creation. (Ex. h2 to h6)
    collisionSuffix: 'v' # A suffix that is prepended to the number given if the ID is repeated.
    permalink: true # If true, creates an anchor tag with a permalink besides the heading.
    permalinkClass: header-anchor # Class used for the permalink anchor tag.
    permalinkSymbol: ¶ # The symbol used to make the permalink.
 ```    

***

### Document

<div style="text-align: center;">
*Coming Soon™*
</div>

***

### Inspired Model
This Theme is based [Daily](https://github.com/GallenHu/hexo-theme-Daily) by [GallenHu](https://github.com/GallenHu)
