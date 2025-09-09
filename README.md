# Real Estate Investment Blog

A Jekyll-powered blog focused on real estate investment analysis, particularly in the Japanese market.

## Setup Instructions

1. **Fork this repository** to your GitHub account
2. **Rename the repository** to `username.github.io` (replace "username" with your GitHub username)
3. **Update the configuration**:
   - Edit `_config.yml` and replace placeholder values:
     - Change `url` to `https://yourusername.github.io`
     - Update author information
     - Customize title and description
4. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Click Save

## Local Development

To run this blog locally:

```bash
# Install Ruby and Bundler first, then:
bundle install
bundle exec jekyll serve
```

Visit `http://localhost:4000` to view your site.

## Adding New Posts

Create new posts in the `_posts` directory with the format:
```
YYYY-MM-DD-title-of-post.md
```

Each post should include front matter:
```yaml
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD
categories: [category1, category2]
tags: [tag1, tag2]
---
```

## Features

- Jekyll-powered static site
- GitHub Pages compatible
- SEO optimized
- RSS feed
- Mobile responsive (using Minima theme)
- Categories and tags support

## Customization

- Modify `_config.yml` for site-wide settings
- Edit `about.md` to customize the About page
- Update the home page by editing `index.md`
- Customize styling by overriding the Minima theme

## Structure

```
├── _config.yml          # Site configuration
├── _posts/              # Blog posts
├── Gemfile              # Ruby dependencies
├── index.md             # Home page
├── about.md             # About page
└── README.md            # This file
```

## GitHub Pages Deployment

Once you push to GitHub, your site will be automatically built and deployed at `https://yourusername.github.io`. Updates typically take a few minutes to appear.

## Support

For Jekyll documentation: https://jekyllrb.com/
For GitHub Pages help: https://docs.github.com/en/pages
