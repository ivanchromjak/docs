---
title: Plugin Setup
icon: settings
toc: true
---

### Creating Knowledge Base Articles
To create a Knowledge Base posts go to `K​nowledge Base > Add New​`, enter title, post content and click Publish button to save. Knowledge Base plugin best displays posts grouped into categories. T​ags​ can also be assigned to posts. Create categories under `K​nowledge Base > Categories`​ and assign post to these categories.

{% include image.html img="Add_New_Article.png" alt="Add New Article" %}

### Setting Up Main Knowledge Base Page
There are two options to display the main knowledge base content, using Gutenberg blocks (recommended) or shortcodes.

#### Gutenberg Blocks
This requires WordPress version 5 or above. Create a page under `P​ages > Add New​`, then the plus icon to add the `Knowledge Base` block and optional search or widget area blocks and save the page.

{% include image.html img="gutenberg_blocks.png" alt="Gutenberg blocks" %}

#### Shortcode
Create a page under `P​ages > Add New​`, then add `[pakb_knowledgebase]` shortcode to its content. Optional `[pakb_search]` shortcode can be used to display search. See shortcodes section for a complete list of shortcodes and their attributes. 

### Horizontal Widget Area
Displays a horizontal widget area on the main knowledge base page, widgets can be added under ​`Appearance > Widgets`. Add the widget area to a page using Gutenberg blocks + button.

### Theme Sidebars
The plugin displays it content by overriding theme’s page template content, by default the plugin overrides `page.php` template file. If your theme has additional page templates, for example full width page template you can select the template under `Knowledge Base > General > Page Template` a​nd knowledge base plugin will use this template for its pages.

### Plugin Options
Plugin options settings are located under `Knowledge Base` menu in dashboard. ​

### Drag & Drop Knowledge Base Reorder
Navigate to `Knowledge Base > General`​ and set `Content Order` setting to `Drag and Drop`. Now you can reorder knowledge base posts and categories using drag and drop under `K​nowledge Base > All Articles` and `K​nowledge Base > Categories`. ​

### Article Voting
Allow users to leave feedback on articles by displaying Like / Dislike voting button under each content on single article page. Enable voting under `Knowledge Base > Voting`. Vote counts for each article can be found under `​Knowledge Base > All Knowledge Base` page.

### Shortcodes

#### Display List Of Knowledge Base Articles
`[pakb_articles posts_per_page="10" orderby="date" order="DESC"]`

| Option | Description | Choices | Default |
| --- | --- | --- | --- |
| posts_per_page | Number of articles to show | integer | 10 |
| orderby | Sort articles by ID, title, date, drag & drop reorder, likes| ID, title, date, menu_order | meta_value_num |
| order | Designates the ascending or descending order of the articles | ASC, DESC | DESC |
| filter | Filter by tag or category | tag, category |
| category | Category ID for category filter |integer |
| tag | Tag ID for tag filter |integer |

#### Display List Of Knowledge Base Categories
`[pakb_categories count="true" orderby="name" order="ASC" number="5"]`

| Option | Description | Choices | Default |
| --- | --- | --- | --- |
| number | Number of categories to show | integer | 10 |
| orderby | Sort categories by name or drag & drop reorder| name, term_group | name |
| order | Designates the ascending or descending order of the categories | ASC, DESC | ASC |
| count | Display article count | true, false | false |

#### Display Knowledge Base main Page
`[pakb_knowledgebase]`

#### Display Search
`[pakb_search]`

#### Display Attachments
`[pakb_attachments]`
Add to a knowledge base article that contain file attachments. Instead of using this shortcode display of attachments can be enabled globally for all articles in plugin options under `Knowledge Base > Single` page. 

### Adding Knowledge Base Widgets
Plugin has three widgets: ​Knowledge Base Search, Knowledge Base Categories​ and Knowledge Base Articles.​ To setup a widgets navigate to ​`Appearance > Widgets`​ and use the drag and drop interface to drop the widget into the desired theme sidebar area.
