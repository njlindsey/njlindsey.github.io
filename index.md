---
title: "Home"
summary: "About this page."
date: 2016-04-13
layout: default
---

## Research Statement
My research focuses on processes that are relevant to humans. I am interested in original observations of Earth signals, and the hypotheses that motivate them. I use a new type of distributed seismic sensor called distributed acoustic sensing to study earthquakes, seismic wave propagation, urban ambient noise sources, soil-rock-water interactions, and permafrost thaw.

## News
12/08 Nate interviewed by PhysicsToday [this cheatsheet](http://ricostacruz.com/cheatsheets/markdown.html)
11/01 GRL [this quick guide](https://milanaryal.com/2015/writing-on-github-pages-and-jekyll-using-markdown/).

###

```
{% raw %}{% for item in page.experience %}
	Various HTML code...
{% endfor %}{% endraw %}
```

To whatever you name the list.

### Editors
In order of most recommended for this workflow:

- [Prose](http://prose.io/#about): "Simple content authoring environment for CMS-free websites", very easy to use for editing GitHub Pages.
	- Direct editing, only requires GitHub authorization.
- [StackEdit](https://stackedit.io/): Elegant interface with live preview and extensive features.
	- Can publish to GitHub, saves documents in local browser storage or the cloud.
- [DraftIn](http://docs.withdraft.com/): Also elegant and easy-to-use interface with extensive features.
	- Requires signup (e-mail).
	- Handy [Chrome extension](https://chrome.google.com/webstore/detail/draft/amlbbbgcijmiooecobhkjblcdkjldmdk) for editing text on any website.

Or just edit pages directly on GitHub.

#### Including files on pages
PDF-files can be linked to from the GitHub Repository, but it is far easier to upload it to [Google Drive](https://drive.google.com/drive/) and embed it (or any other cloud storage that generates an `<iframe>`-embed tag).

Procedure (from [here](http://www.steegle.com/websites/google-sites-howtos/embed-drive-pdf)):

1. Find the PDF file in Google Drive.
2. Preview the PDF file in Google Drive.
3. Pop-out the Google Drive preview.
4. Use the More actions menu and choose Embed item.
5. Copy code provided.
6. Paste it on a separate line in the Markdown-file, like this:

```
Paragraph...

<iframe style="margin: 10px 0 40px 0;" class="pdf-iframe" src="https://drive.google.com/file/d/0B-xXQEsWEjrUUmpBdkhIVS10YjA/preview" width="100%" height="768"></iframe>

Other Markdown and text.
```

#### Site settings
The links in the menu, and their order, are edited through `_config.yml`. The format is also nested YAML lists, like the FrontMatter described above. **'baseurl' must be set to your repository (eg. `baseurl: username.github.io`), or the build will fail.** The `name` and `description` variable should also be set, as well as `mathjax: true` if you need to render MathJax formulas on pages.

The `markdown, encoding, locale` variables **should not be changed**.

To find the right page-link (`#somethingonthepage`) you open the page, hover a heading so that the icon-link displays, right-click it and choose "Copy link". Everything after the `#` is the link for this specific title on the page.

Note that these links must be encapsulated in quotes in the lists in `_config.yml`, or they will be interpreted as code-comments.

### Development
Written in [Jekyll](http://jekyllrb.com/), structured with [Bootstrap v4](http://getbootstrap.com/), styled with [plain CSS](http://www.css3-tutorial.net/introduction/what-is-css/). The Jekyll-output (in the `_site`-folder when generated) can be hosted anywhere (static files). For further development, see [Jekyll Tips](http://jekyll.tips/) and [GitHub Pages Setup Guide](http://jmcglone.com/guides/github-pages/).
