# DisCouRSE Network Project Website

Please do submit pull requests to update or improve content as needed.


## Building locally

For testing more substantial changes, it's helpful to be able to view the site locally rather than just looking at the sources.
Here I describe in brief how I got this working on my Mac.

1. Install Ruby, e.g. `brew install ruby`

2. Delete any old `Gemfile.lock` file to avoid potential conflicts

3. Install Jekyll and dependencies using `bundle`, e.g. `/opt/homebrew/opt/ruby/bin/bundle install`

4. Use `bundle` to build the site too: `/opt/homebrew/opt/ruby/bin/bundle exec jekyll serve --baseurl=""`

It will automatically re-build whenever changes to the website files are saved,
and by default makes the site available at http://127.0.0.1:4000/


## Minimal Mistakes theme troubleshooting

This is made with the [Minimal Mistakes Jekyll theme](https://github.com/mmistakes/minimal-mistakes).

[Theme documentation is available](https://mmistakes.github.io/minimal-mistakes/docs/).

If you have a question about using Jekyll, start a discussion on the [Jekyll Forum](https://talk.jekyllrb.com/) or [StackOverflow](https://stackoverflow.com/questions/tagged/jekyll). Other resources:

- [Ruby 101](https://jekyllrb.com/docs/ruby-101/)
- [Setting up a Jekyll site with GitHub Pages](https://jekyllrb.com/docs/github-pages/)
- [Configuring GitHub Metadata](https://github.com/jekyll/github-metadata/blob/master/docs/configuration.md#configuration) to work properly when developing locally and avoid `No GitHub API authentication could be found. Some fields may be missing or have incorrect data.` warnings.
