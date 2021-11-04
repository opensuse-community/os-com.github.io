# Welcome at openSUSE-Community!

This GitHub repository provides the source for the [openSUSE community website](https://www.opensuse-community.org) which provides public-facing documentation and  one-click installers for multimedia codecs and more.

It is a combination of Markdown, HTML, CSS which is rendered by [Jekyll](https://jekyllrb.com/).

The [page](https://www.opensuse-community.org/) and it's content is provided by members of the openSUSE community. While we welcome the openness and open source base of our [favorite distribution](https://www.opensuse.org/), we also want to make the lives of our community easy and smooth: therefor, we provide a simple way to install the needed software which can not be provided directly by openSUSE.

## Testing and development

1) install needed packages
For local builds, please install [bundler](https://rubygems.org/gems/bundler), [Jekyll](https://jekyllrb.com/) and the development headers for Ruby:

```zypper in 'rubygem(bundler)' 'rubygem(jekyll)' ruby-devel```

> Note: on Leap 15.3, you might run in a dependency problem. Accept to install jekyll ignoring the problem - and install `zypper in 'rubygem(terminal-table)'` separately.

2) download themes and other gems

Once the core packages are installed successfully, please run: `bundle update github-pages`

3) run jekyll

Now everything should be fine to run `bundle exec jekyll serve`

4) open your browser

Visit http://127.0.0.1:4000/ in your local browser. You should see the generated pages. Have a look at your console for error messages.

5) change something

Usually (as long as you don't interrupt the jekyll process), you should be able to do some changes - and jekyll will directly render the page and make your changes visible in your local browser.

6) commit and push back

Once you are happy with your changes, commit them locally via `git commit -a`. If everything is done, feel free to either commit them back directly (`git push`) or create a merge request via the standard Github way.


