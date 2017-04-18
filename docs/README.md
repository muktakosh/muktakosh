# Muktakosh.org source

This is the source code for Muktakosh.org website and blog. It is a static website built using Jekyll and deployed and hosted using Github Pages. This directory serves as the root for Jekyll. Github Pages is configured to compile this directory on the `master` branch. The website uses Foundation 6 for theming and Fontawesome Icons for the icons.

Note: This file is ignored by Jekyll and is not included in the final output.

## Directory structure

These are the important files and subdirectories:

- **`_posts/`** - Contains the blog post sources.
- **`_theme/`** - Contains theme layouts, includes, SASS and vendor assets
    - **`_theme/_vendors/`** - Installation directory for Bower packages
- **`assets/`** - Contains site-specific custom assets
- **`blog/index.html`** - Landing and pagination handler for Blog
- **`index.html`** - Homepage

## Adding/editing content

### Writing a blog post

- Create a Markdown file in `_posts/` following Jekyll conventions. You can copy template post from [`_posts/_2006-12-22-template.md`][template] to `_posts/YYYY-MM-DD-your-post-slug.md`, without leading underscore. See [writing posts in Jekyll][jekyll-post] for details.
- Set `layout: post` in the front matter.
- Put cover image for the blog post in `_assets/images/covers/` and update the `image:` field in the front matter of your post to reflect the file name.
- Write your post.

### Create a new page

- Create a file with front matter, preferably with the `.md` extension. Look at [`about.md`][about-file] for an example.
- Keep `layout: page` in the front matter of the page.

[template]: _posts/_2006-12-22-template.md
[jekyll-post]: https://jekyllrb.com/docs/posts/
[about-file]: about.md
