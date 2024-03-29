---
title: Lite Helpdesk Jekyll Theme
cta:
  # - title: Contact Support
  #   icon: lifesaver
  #   url: https://themeforest.net/item/guia-helpdesk-and-documentation-html5-responsive-template/25254625/support
  # - title: Learn Jekyll
  #   icon: album
  #   url: https://themeforest.net/item/guia-helpdesk-and-documentation-html5-responsive-template/25254625/support
  - title: Customization Services
    icon: code
    url: https://unbound.studio/contact/
---

#### Table of contents
{:.no_toc}
* TOC
{:toc}
{:.uk-list}

## Installation

Install the dependencies with [Bundler](http://bundler.io/):

```bash
bundle install
```

Run the following to generate your site:
```bash
bundle exec jekyll serve
```

You can find more on [Deployment Methods](https://jekyllrb.com/docs/deployment-methods/) page on Jekyll website.

### Google analytics

To enable Google Anaytics, add the following lines to your Jekyll site:

```yaml
  google_analytics: UA-NNNNNNNN-N
```

Google Analytics will only appear in production, i.e., `JEKYLL_ENV=production`

### Updating favicon

You can find the current favicon (favicon.png) inside the theme `/assets/img/` directory, just replace it with your new favicon.

## Home Page

To create a home page, just create a `index.md` file inside the root directory. The following is a YAML Front Matter example for a page:

```yaml
---
layout: home
hero:
  title: How Can We Help?
  subtitle: SELF SERVICE KNOWLEDGE BASE
cta:
  title: Didn't find an answer to your question?
  button_text: Contact Us   
  button_url: /contact/
filter: true
---
```

Home page category boxes are added in `_data/navigation_home.yml`, e.g.:
```yml
- title: Getting Started
  desc: Get your account up and running in just few easy steps
  icon: settings
  doc: usage

- title: Account and Billing
  desc: Managing your account, creating new users and exporting data
  icon: credit-card
  doc: drafts
```

All available icons can be found [here](https://getuikit.com/docs/icon#library).

## Support Posts

Create new support post entries in `_support` folder, similar to creating posts, only the title is required in front matter:

```yml
---
title: Category hosting Setting up new domain and page
---
```

### Adding Table of contents
Add the following to the front matter of the support post:
```
toc: true
```

## Changelog page

Create  new page with the following front matter:

```yml
---
layout: changelog
title: Changelog
permalink: /changelog/
---
```

Changelog enties are added in `_data/changelog.yml`:

```yml
- title: Version 0.6.0
  date: Aug 15, 2017
  list:
  - Added style support for radio and checkbox in Firefox
  - Removed class from Section component
```

## Contact Form (via FormSpree)

To display Google map on contact page, add the following in your page content, replacing latitude, longitude and zoom values:

Submit the form and confirm your email address at [FormSpree](https://formspree.io/). Then add the following include to a page, replacing the email address:

```yaml
{% include formspree.html email="john@company.com" redirect="/thanks" %}
```

## Content

### Google Map

To display Google map on contact page, add the following in your page content, replacing latitude, longitude and zoom values:

```yaml
{% include map.html latitude="40.6700" longitude="-73.9400" zoom="16" %}
```

### Images
To keep things more organized, add post images to `/assets/posts/` directory, and add theme images to `/assets/img/` directory.

To add an image to a post or page use the following:
Local image from `/assets/posts/` directory:
```yaml
{% include image.html img="girl.jpg" alt="Alt for image" caption="Girl on a rock" %}
```
External image in lightbox:
```yaml
{% include image.html img="https://source.unsplash.com/TT-ROxWj9nA.jpg" lightbox="true" alt="Alt for image" caption="Image in lightbox" %}
```


### Videos
Embed local videos:
```html
<video controls playsinline uk-video="automute: true">
    <source src="http://www.quirksmode.org/html5/videos/big_buck_bunny.mp4" type="video/mp4">
    <source src="http://www.quirksmode.org/html5/videos/big_buck_bunny.ogv" type="video/ogg">
</video>
```
Embed YouTube videos:
```html
<iframe src="http://www.youtube.com/embed/YE7VzlLtp-4?autoplay=0&amp;showinfo=0&amp;rel=0&amp;modestbranding=1&amp;playsinline=1" width="600" height="340" frameborder="0" allowfullscreen uk-responsive uk-video="automute: true"></iframe>
```

### Comments

Optionally, if you have a Disqus account, you can tell Jekyll to use it to show a comments section below each blog post. To enable it, add the following lines to your Jekyll site:

```yaml
disqus:
    shortname: my_disqus_shortname
```

You can find out more about Disqus' shortnames [here](https://help.disqus.com/customer/portal/articles/466208).

Comments are enabled by default and will only appear in production, i.e., `JEKYLL_ENV=production`. If you don't want to display comments for a particular post you can disable them by adding `comments: false` to that post's YAML Front Matter.


## Development

Install [UIkit](https://getuikit.com/) font end framework dependency via Npm:
```bash
npm install
```
Enable live browser reload with the following:
```bash
bundle exec jekyll s --livereload
```

### Customization

To modify the primary color, open `/_sass/theme/variables.scss` and replace the color values e.g.:

```scss
// Primary color
$tm-primary-color: #0089ff;
// Body background
$tm-body-background: linear-gradient(to top, #0065fd 0%, #0089ff 100%);
```

Further style customisation can be done in the following files:
```
/_sass/theme/mixins.scss
/_sass/theme/variables.scss
```

## Credits

- Google analytics https://www.google.com/analytics/
- Google maps https://www.google.com/maps
- UIkit front end framework https://getuikit.com/
- Jekyll https://jekyllrb.com/
- FormSpree https://formspree.io/

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