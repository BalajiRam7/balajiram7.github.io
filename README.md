# Balaji Ramachandran — Personal Academic Website

Jekyll-powered GitHub Pages site for Balaji Ramachandran.

## Local development

This project uses Ruby 3.3 and Jekyll. With Homebrew on macOS:

```bash
brew install ruby@3.3
export PATH="$(brew --prefix ruby@3.3)/bin:$PATH"
gem install bundler
bundle install
bundle exec jekyll serve
```

Open `http://localhost:4000` to preview the site. Do not use a plain static HTTP server because it will not process Jekyll front matter or Liquid templates.

## Publish

Push the contents of this directory to the `balajiram.github.io` repository and enable GitHub Pages from the repository's main branch. GitHub Pages builds the site with Jekyll.

## Included

- Reusable Jekyll layout with a structured academic homepage
- Research, publications, experience, and education sections
- Dedicated blog page powered by Jekyll posts in `_posts`
- Links to Google Scholar, LinkedIn, arXiv, and email
- Responsive layout with a small-screen navigation menu
