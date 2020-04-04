---
title: Yogee Yoga & Meditation Studio HTML Template
cta:
  # - title: Contact Support
  #   icon: lifesaver
  #   url: https://themeforest.net/user/unboundstudio
  # - title: Learn Jekyll
  #   icon: album
  #   url: https://themeforest.net/user/unboundstudio
  - title: Customization Services
    icon: code
    url: https://unbound.studio/contact/
---

#### Table of contents
{:.no_toc}
* TOC
{:toc}
{:.uk-list}

## Folder Structure
Within the template you'll find the following folders:

`/dist`    (production ready HTML/CSS/JS files)  
`/src`     (SASS/JS source files when using build process)


## HTML Structure
This responsive theme built with on UIkit 3.2 so please refer to original docs for more info and components use [https://getuikit.com/docs/introduction](https://getuikit.com/docs/introduction).

The template consists of:

`dist/index.html` - Home page  

### Navigation
Header navigation link are located within the `<nav>` tag, active page link has `"uk-active"` class assigned dynamically using scrollspy JS.

### Footer
Copyright can be edited inside the `<footer>` tag:
Social icon link example:
```
<a href="https://www.instagram.com/" data-uk-icon="icon: instagram" class="uk-icon-link"></a>
```

All available icons are documented here: [https://getuikit.com/docs/icon](https://getuikit.com/docs/icon).

## CSS File and Structure
To modify the look and feel of the template, edit the SASS files located in `src/scss/` folder. 
```
src/scss/main.scss - Main template styles file that imports partial SASS files
```

If you would like to edit a specific Uikit component, you can either: 
override SASS variables in `src/scss/_variables.scss`
or modify/create a custom class in `src/scss/_mixins.scss`.

For the list of all available variables and mixins in Uikit see the following files:
`node_modules/uikit/src/scss/variables.scss`  
`node_modules/uikit/src/scss/mixins.scss`  

## Using Build Process
We used CodeKit [https://codekitapp.com/](https://codekitapp.com/) and Npm [https://www.npmjs.com/](https://www.npmjs.com/) for build process.
Run the following npm commands using terminal in root template directory:

`npm install`   (run once to install UIKit and awesomplete dependencies)

Note: npm must be first installed globally, see npm site [https://www.npmjs.com/](https://www.npmjs.com/).
CodeKit is then used to compile template source files (KIT/SASS/JS) in root folder.

## JavaScript
The following scripts are loaded before the body closing tag:

The following script is loaded head tag:

`dist/js/uikit.js` - Contains main UIkit scripts and icons
`dist/js/custom.js` - Contains datepicker script, also add your custom Javascript here. Datepicker documentation can be hound here [https://github.com/qodesmith/datepicker](https://github.com/qodesmith/datepicker).

Detailed UIkit script documentation is located here [https://getuikit.com/docs/javascript](https://getuikit.com/docs/javascript).


## Manually Overriding Files
If you decide to manually modify CSS/JS files (not recommended) use `/dist` folder. If you would like to edit a specific component of the site, simply check the table of contents in the `main.css` template  file, and then scroll down until you find the appropriate style that needs to be edited.

If you would like to edit the primary color of the theme you should do "Replace all" color `#e7e87c` with the desired one.

## Framework
Template uses UIkit front-end framework version 3, documentation is located here: [https://getuikit.com/docs/introduction](https://getuikit.com/docs/introduction).

## Support
Depending on where you purchased the product, contact us:

- Creative Market: Contact us through "Ask a question" button on the products page on Creative Market
- Gumroad: The purchase receipt contains our contact email address

Customer support is provided for up to six months from the purchase date and is provided Monday to Friday during the business week. We aim to answer all support requests daily, most are handled within 24h.

Before contacting support please:

- Read this documentation
- Describe your problem in detail
- Include links
- Attach screenshot