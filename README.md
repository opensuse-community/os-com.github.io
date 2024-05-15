=======
# Welcome at openSUSE-Community!

This GitHub repository provides the source for the [openSUSE community
website](https://www.opensuse-community.org) which provides public-facing
documentation and  one-click installers for multimedia codecs and more.

It is a combination of Markdown, HTML, CSS which is rendered by
[Jekyll](https://jekyllrb.com/).

The [page](https://www.opensuse-community.org/) and it's content is provided by
members of the openSUSE community. While we welcome the openness and open
source base of our [favorite distribution](https://www.opensuse.org/), we also
want to make the lives of our community easy and smooth: therefor, we provide a
simple way to install the needed software which can not be provided directly by
openSUSE.

## Help! I am lost!

* [Markdown Reference][1]
* [Wiki specific examples][2]


# Testing and development

## Setting up your environment

1. install docker: ```zypper install docker```
2. run docker: ```systemctl enable --now docker```
3. make sure, your $user is in the docker group: ```groupmod -a -U $user docker```
4. checkout the GIT repo: ```git clone git@github.com:opensuse-community/os-com.github.io.git```
5. copy the template: ```cp -v docker-compose.override.yml.example docker-compose.override.yml```
6. adjust the template to your needs (set 'JEKYLL_UID' and 'JEKYLL_GID' to your $user IDs)
6. start the container: ```docker-compose up```
7. access the page at http://localhost:4000
8. edit the files and enjoy
9. don't forget to submit back: ```git commit -m "I made the world better" -a && git push``` ;-)

Happy documentation writing.

[1]: https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/setting-a-markdown-processor-for-your-github-pages-site-using-jekyll
[2]: https://www.markdownguide.org/tools/github-pages/

