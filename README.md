# Cards World (عالم البطاقات)

A simple Hugo site for my son Taymullah that serves as a knowledge base of animals and other things he is learning about.

**Live site:** https://cards.amersaw.info

## Getting Started

### Prerequisites

- [Hugo](https://gohugo.io/installation/) (extended edition)

### Run locally

```bash
hugo server -D
```

### Build

```bash
hugo build
```

The site will be generated in the `public/` directory.

## Content

Cards are organized by category. Each category is a folder under `content/` with an `_index.md` and individual card markdown files.

### Adding a new card

Create a markdown file under the appropriate category folder:

```bash
hugo new content <category>/<card-name>.md
```

Then populate the front matter with attributes like `scientific_name`, `length`, `mass`, `image`, etc.

### Adding a new category

Create a new folder under `content/` with an `_index.md` containing:

```yaml
---
title: "Category Name"
description: "Short description"
image: "images/category-image.jpg"
icon: "🎯"
weight: 1
---
```
