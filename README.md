Remark Czech Preprocessor
=========================
A plugin for the [Remark Markdown processor](https://remark.js.org/),
which is intended to enhance Czech typography for the web, mostly by adding
hyphenation.

Originally intended to be used on [Gatsby](https://www.gatsbyjs.com/) sources.

**Note: This plugin is not yet published on NPM.**

What it does
------------
* Adds hyphenation in the form of `&shy;` characters. This is necessary
  for text justification.
* Adds `&nbsp;` before one-letter prepositions.