# Sean’s blog

This repository powers [sboots.ca](https://sboots.ca/).

It uses [Hugo](https://gohugo.io) and the [Hugo Bootstrap v4 Blog](https://github.com/alanorth/hugo-theme-bootstrap4-blog) theme by [Alan Orth](https://github.com/alanorth).

The code here is licensed under the [MIT License](https://github.com/sboots/sboots.ca/blob/master/LICENSE). The v4 Blog theme is licensed under the [Creative Commons Attribution 3.0 license](https://github.com/alanorth/hugo-theme-bootstrap4-blog/blob/master/LICENSE.txt). 

Content on the blog is licensed under the [Creative Commons Attribution 4.0 International license](https://creativecommons.org/licenses/by/4.0/). That means you can share and adapt the material, provided you give appropriate credit and indicate if changes were made.

Feel free to reuse the code here, and to reshare post content (with attribution) as you’d like!

## Local development

### First run

To build this site locally, clone it into a new folder.

Then, from that folder, run

```
git submodule update --init --recursive
```

to pull in the theme submodule.

### Local preview

To display draft posts (and re-render styles and layouts each time), run

```
hugo server -D --disableFastRender
```

If you have questions or comments, please don’t hesitate to reach out here or [on Twitter](https://twitter.com/sboots)!
