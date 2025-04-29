# LinuxArtistry - Klejdi's Blog & Portfolio

This is a personal home site for Klejdi (Klej) that combines blogging functionality with a carrd.io-style introduction page. The site focuses on Linux and art content, featuring a terminal-inspired theme that reflects the Linux aesthetic while maintaining visual appeal for showcasing artistic content.

## Features

- Clean, responsive design inspired by terminal interfaces
- Blog section for technical articles about Linux and art
- Portfolio section for showcasing projects
- Dark/light theme support with automatic OS preference detection
- Contact form (static demo)

## Static Site Structure

The generated static site contains:

- `index.html` - Main landing page with all sections
- `/blog/` - Individual blog post pages
- `/portfolio/` - Individual portfolio project pages
- `index.css` - Styling for the entire site

## Adding New Content

### Adding a Blog Post

1. Create a new Markdown file in the `blogs/` directory with the format:

```markdown
---
title: "Your Blog Post Title"
date: "YYYY-MM-DD"
category: "Linux"
excerpt: "A brief description of your post"
imageUrl: "https://example.com/your-image.jpg"
slug: "your-unique-slug"
---

# Your Blog Post Title

Your content here...
```

2. Run `node build.js` to regenerate the site

### Adding a Portfolio Item

1. Create a new Markdown file in the `portfolio/` directory with the format:

```markdown
---
title: "Your Project Title"
category: "Digital Art"
imageUrl: "https://example.com/your-image.jpg"
description: "A brief description of your project"
slug: "your-unique-slug"
---

# Your Project Title

Project content here...
```

2. Run `node build.js` to regenerate the site

## Deploying to GitHub Pages

1. Create a new GitHub repository
2. Upload the contents of the `dist` directory to your repository 
3. Go to the repository settings → Pages
4. Configure the source as your main branch (or a specific folder)
5. Your site will be available at `https://your-username.github.io/your-repo-name/`

## Local Development

To work on this site locally:

1. Clone the repository
2. Run `npm install` to install dependencies
3. Edit the Markdown files in `blogs/` and `portfolio/` directories
4. Run `node build.js` to build the site
5. The generated site will be in the `dist/` directory
