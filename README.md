Remark Czech Preprocessor
=========================
A plugin for the [Remark Markdown processor](https://remark.js.org/),
which is intended to enhance Czech typography for the web, mostly by adding
hyphenation.

Originally intended to be used on [Gatsby](https://www.gatsbyjs.com/) sources.

What it does
------------
* Adds hyphenation in the form of `&shy;` characters. This is necessary
  for text justification.
* Adds `&nbsp;` before one-letter prepositions.

Usage
-----
**Note: This plugin is not yet published on NPM.**
You can install it from github.

```
$ yarn add -E tomvej/remark-czech-preprocessor
```

Use it as a Remark plugin, e.g. in `gatsby-config.js`:
```
module.exports = {
    plugins: [
        {
            resolve: 'gatsby-transformer-remark',
            options: {
                plugins: ['remark-czech-preprocessor'],
            },
        },
    ],
};
```

You can then switch on hyphenation in css:
```css
p {
  text-align: justify;
  hyphens: manual;
}
```