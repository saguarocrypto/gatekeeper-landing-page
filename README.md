# Saguaro Landing Page & Blog

This is the official website for Saguaro, featuring our MEV protection solution **Gatekeeper** for Solana, built with Jekyll and hosted on GitHub Pages.

## 🚀 Quick Start

### Prerequisites
- Ruby (version 2.7 or higher)
- Bundler gem

### Local Development

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd gatekeeper-landing-page
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Run locally**
   ```bash
   bundle exec jekyll serve
   ```
   
   Your site will be available at `http://localhost:4000`

4. **Run with live reload (optional)**
   ```bash
   bundle exec jekyll serve --livereload
   ```

## 📝 Writing Blog Posts

### Creating a New Post

1. Create a new file in the `_posts` folder with the format: `YYYY-MM-DD-your-post-title.md`

2. Add the front matter at the top:
   ```yaml
   ---
   layout: post
   title: "Your Post Title"
   date: 2025-01-26 10:00:00 -0800
   author: "Your Name"
   tags: [tag1, tag2, tag3]
   excerpt: "A brief description of your post that appears in the blog listing."
   ---
   ```

3. Write your content in Markdown below the front matter.

### Markdown Examples

```markdown
# Main Heading
## Sub Heading
### Smaller Heading

**Bold text** and *italic text*

- Bullet point 1
- Bullet point 2

1. Numbered list item 1
2. Numbered list item 2

> This is a blockquote

`Inline code` and:

```
Code blocks
```

[Link text](https://example.com)
```

### Adding Images

1. Add your images to the `assets/images/` folder
2. Reference them in your posts:
   ```markdown
   ![Alt text]({{ '/assets/images/your-image.png' | relative_url }})
   ```

## 🎨 Customization

### Site Configuration
Edit `_config.yml` to update:
- Site title and description
- URL and baseurl
- Social media links
- Other site-wide settings

### Styling
- Main styles are in `assets/css/style.css`
- The site uses CSS custom properties (variables) for easy theming
- Colors, fonts, and spacing can be modified in the `:root` section

### Navigation
Update the navigation links in `_layouts/default.html` if you want to add new pages.

## 🚀 Deployment

### GitHub Pages (Automatic)

This site is configured to deploy automatically to GitHub Pages when you push to the main branch.

1. **Enable GitHub Pages**
   - Go to your repository settings
   - Scroll to "Pages" section
   - Set source to "GitHub Actions"

2. **Push your changes**
   ```bash
   git add .
   git commit -m "Add new blog post"
   git push origin main
   ```

3. **Your site will be live at**: `https://yourusername.github.io/your-repo-name`

### Manual Deployment

If you want to deploy elsewhere:
```bash
bundle exec jekyll build
```
This creates a `_site` folder with your static files.

## 📁 Project Structure

```
├── _config.yml          # Jekyll configuration
├── _layouts/            # Page templates
│   ├── default.html     # Base layout
│   └── post.html        # Blog post layout
├── _posts/              # Blog posts (Markdown files)
├── assets/
│   ├── css/
│   │   └── style.css    # Main stylesheet
│   └── images/          # Image files
├── blog/
│   └── index.html       # Blog listing page
├── index.md             # Homepage
├── team.md              # Team page
├── Gemfile              # Ruby dependencies
└── README.md            # This file
```

## 🛠️ Development Tips

### Local Testing
- Always test locally before pushing
- Use `bundle exec jekyll serve --drafts` to preview draft posts
- Check that all links work and images load properly

### Writing Tips
- Use descriptive titles and excerpts
- Add relevant tags to help organize content
- Include images to make posts more engaging
- Keep paragraphs short for better readability

### Performance
- Optimize images before adding them
- Use appropriate image formats (WebP for modern browsers)
- Keep the number of plugins minimal

## 🎯 SEO Features

The site includes several SEO optimizations:
- Semantic HTML structure
- Meta tags and Open Graph tags
- XML sitemap generation
- RSS feed
- Structured data for blog posts

## 📱 Responsive Design

The site is fully responsive and works well on:
- Desktop computers
- Tablets
- Mobile phones

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test locally
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

Built with ❤️ using Jekyll and GitHub Pages 