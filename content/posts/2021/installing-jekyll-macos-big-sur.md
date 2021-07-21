---
title: "Installing Jekyll locally on MacOS Big Sur"
date: 2021-07-20T17:02:32-07:00
summary: "Our team often uses Jekyll and GitHub Pages to build micro-sites for project documentation. I recently set up Jekyll for the first time in a while on a new computer, which involves getting Ruby and the Bundler package manager to work happily. Here are the steps I used."
images: []
---

Our team often uses [Jekyll](https://jekyllrb.com/) and [GitHub Pages](https://pages.github.com/) to build [micro-sites for project documentation](https://github.com/cds-snc?q=documentation&type=&language=&sort=). Jekyll is a [static website builder](https://jamstack.org/generators/), which makes it easy to build and deploy essentially indestructible (although usually not interactive) websites. Similar tools include [Hugo](https://gohugo.io/) (my go-to for [most](https://meetingcostcalculator.ca/) [civic](https://large-government-of-canada-it-projects.github.io/) [tech](https://internal-red-tape-reduction-report.github.io/) [projects](https://goc-spending.github.io/)), [Gatsby](https://www.gatsbyjs.com/) (which powers “[Is this blocked in my department?](https://isthisblockedinmydepartment.ca/)”), and [Eleventy](https://www.11ty.dev/) (which I’ve only used [once](https://shoulditbeblockedinmydepartment.ca/), but found really easy to use). Jekyll is the <abbr title="original gangster">OG</abbr> of static websites and it’s a bit dated nowadays, but GitHub Pages’ built-in support for it is really handy. 

I recently set up Jekyll for the first time in a while on a new computer, which involves getting Ruby and the Bundler package manager to work happily. Here are the steps I used.

(Note that this is for a fresh install on a new Mac, using the default zsh shell; if you’ve upgraded to Big Sur and have older Ruby versions or packages installed, you may want to follow the steps [here](https://jekyllrb.com/docs/installation/macos/) or [here](https://www.moncefbelyamani.com/the-definitive-guide-to-installing-ruby-gems-on-a-mac/) to use Homebrew, rvm, or another installation method.)

## Installation steps

1\. Clone the static website repository you’re working on, and `cd` into that folder.

2\. Check that a new enough version of Ruby is installed to meet [Jekyll’s system requirements](https://jekyllrb.com/docs/installation/#requirements):

```
ruby -v
```

The version of Ruby included with Big Sur (currently 2.6.0) is recent enough; good to go there.

3\. In the past, I’ve installed Ruby gems using sudo, as part of the system Ruby installation. That’s [no longer recommended](https://stackoverflow.com/a/59721772), so instead I did the following:

```
gem install --user-install bundler jekyll
```

4\. Then, I added Bundler (and other gems) to my path file [following the instructions here](https://jekyllrb.com/docs/installation/macos/#local-install):

```
echo 'export PATH="$HOME/.gem/ruby/2.6.0/bin:$PATH"' >> ~/.zshrc
```

Note that for newer versions of Ruby, you should change `2.6.0` above to match your installed version. If you’re using the Bash shell the syntax is [slightly different](https://jekyllrb.com/docs/installation/macos/#local-install).

5\. Once Bundler was installed, I needed to use a similar approach [to save bundle packages locally](https://stackoverflow.com/a/49719722), rather than in a system-wide location.

From within the website folder, I ran:

```
bundle config set --local path 'vendor/bundle'
```

Which saves packages to a “vendor” directory within the project folder, similar to [Composer](https://getcomposer.org/)’s “vendor” folder or [npm](https://docs.npmjs.com/about-npm)’s “node_modules” folder.

6\. Then, I ran:

```
bundle install
```

7\. Finally, you’ll need to **exclude** that vendor folder from Jekyll’s config file, so that it [doesn’t try to parse and generate webpages from anything recognizable in that vendor folder](https://jekyllrb.com/docs/troubleshooting/#configuration-problems). You can do that by adding a “vendor/” line to the exclude config list, for example:

```
exclude:
- .ruby-gemset
- .ruby-version
- Gemfile
- Gemfile.lock
- Makefile
- README.md
- vendor/
```

8\. You’ll want to add the following lines to your `.gitignore` file as well:

```
vendor/
.bundle/
```

9\. After that, you’re good to run your Jekyll site locally! You can do that with,

```
bundle exec jekyll serve --watch --baseurl ''
```

…although this might vary slightly depending on your Jekyll setup.

Happy Jekyll’ing! 
