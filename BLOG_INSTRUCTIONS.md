# Sageloom Analytics: Publishing Blogs

This file exists in the \`dist\` output directory so it's always accessible. This guide explains how to write and publish a new blog post directly via GitHub.

## Step 1: Create a Markdown (.md) File
1. Go to your repository on GitHub.
2. Navigate to \`src/content/blogs/\`.
3. Click **Add file** > **Create new file**.
4. Name your file with a URL-friendly name (e.g., \`my-first-post.md\`). This filename will become the URL (e.g., \`sageloom.in/blog/my-first-post\`).

## Step 2: Add YAML Frontmatter
At the very top of your new \`.md\` file, you **must** include metadata (called frontmatter) enclosed in \`---\` tags. Copy and paste this template:

```yaml
---
title: "Your Catchy Blog Title Here"
date: "YYYY-MM-DD"
author: "Author Name"
description: "A short 1-2 sentence summary of this post."
---
```

## Step 3: Write Your Content
Below the second \`---\`, write your blog post using standard Markdown!

*   Use \`#\` for headers or \`##\` for subheaders.
*   Use \`**bold**\` or \`*italic*\`.
*   Create bullet points using \`-\` or \`*\`.

## Step 4: Adding Images
1. **Upload the Image**: First, upload your image file (e.g., \`my-chart.png\`) to the \`public/\` folder in your GitHub repository.
2. **Reference the Image**: In your blog markdown file, use the absolute path starting with a forward slash.
   
   Example:
   \`\`\`markdown
   ![Description of the image](/my-chart.png)
   \`\`\`
   *(Do not include \`public\` in the path)*

## Step 5: Publish!
Commit and push your changes to your \`main\` branch. If you have Netlify configured to auto-deploy, your new blog post will automatically appear on the live website within minutes!
