---
title: Sidebar Addon
icon: plus
toc: true
---

### Setup
The addon will automatically display sidebar toggle button on your site after plugin activation with the default settings. Additional addon options settings are located under `Knowledge Base > Sidebar`. 

The site front end will display sidebar toggle button at the bottom right corner.

{% include image.html img="sidebar.png" alt="Sidebar Toggle Button" %}

### Contact Form
To add a contact form to the sidebar install and activate third-party plugin [Contact Form 7](https://wordpress.org/plugins/contact-form-7/).

Next, navigate to Contact menu and copy the form shortcode e.g. `[contact-form-7 id="1040"]`.

Next, navigate to `Knowledge Base > Sidebar` and paste the shortcode inside the Contact Button Shortcode textarea and save settings.

On the front end, open the sidebar and click on Contact button to reveal the form.

### Translation
1. Download and install [Poedit](https://poedit.net/)
2. Open the program after the installation. Click **File > Open** and find the original
`pressapps-­knowledge­-base-sidebar.po` ​file located in the `l​anguages`​ directory in plugin
root.
3. Translate all the words to your language and save your translated file in the same
`languages`​ directory with the name of your language and country codes.
4. If your language is, for example, Russian and the country is Russia, then you must save the file like
this: `​pressapps-­knowledge­-base­-sidebar-ru_RU.po`. ​Use `pressapps-­knowledge­-base­-sidebar`​, then the first parameter is a language code, the second parameter is a country code. All languages codes can be found [here](http://www.gnu.org/software/gettext/manual/gettext.html#Language-Codes).
and all countries codes can be found [here](http://www.gnu.org/software/gettext/manual/gettext.html#Country-Codes).