# manishpunia.com

Personal website for [manishpunia.com](https://manishpunia.com), hosted with GitHub Pages and Jekyll.

## Local Development

Install the locked Bundler version, install dependencies, and serve the site:

```sh
gem install bundler:2.1.4
bundle config set --local path vendor/bundle
bundle install
bundle exec jekyll serve
```

The site uses the So Simple remote theme. Minimal Mistakes and Algolia remain available in the Gemfile for future theme/search work.

## Known Local Setup Issue

The current `Gemfile.lock` is old and may fail during `bundle install` with dependency resolution errors around `github-pages`, `activesupport`, or `kramdown`. GitHub Pages is already serving the site with a newer Pages/Jekyll stack, so the next maintenance pass should refresh `Gemfile.lock` in a modern Ruby environment.
