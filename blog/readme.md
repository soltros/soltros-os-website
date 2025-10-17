# My Blog

A simple, static blog built with the SoltrOS framework.

## How to Add a New Post

1. **Copy the template:**
   ```bash
   cp posts/post-template.html posts/my-new-post.html
   ```

2. **Edit the new file:**
   - Update the `<title>` tag
   - Update the `<meta name="description">` tag
   - Change the `<h1>` post title
   - Update the date and reading time
   - Add/remove tags as needed
   - Write your content in the `.post-content` section

3. **Add to index.html:**
   - Open `index.html`
   - Copy an existing `<article class="post-card">` block
   - Paste it at the top (newest posts first)
   - Update the date, title, excerpt, tags, and link
   - Make sure the `href` matches your new filename

4. **Test locally:**
   - Open `index.html` in your browser
   - Click through to your new post
   - Check that everything looks good

5. **Deploy:**
   ```bash
   git add .
   git commit -m "Add new blog post: [Post Title]"
   git push origin main
   ```

## Quick Writing Tips

- **Images:** Put images in a `posts/images/` folder and reference like: `<img src="images/my-photo.jpg" alt="Description">`
- **Tags:** Keep them consistent. Common ones: Tutorial, Tips, Meta, Announcement
- **Reading Time:** Roughly 200-250 words per minute
- **Excerpts:** Keep them under 150 characters for best display

## Deployment Options

### GitHub Pages
1. Go to repository Settings → Pages
2. Select branch: `main`, folder: `/ (root)`
3. Save and wait a few minutes
4. Your blog will be at: `https://yourusername.github.io/repo-name/`

### Netlify
1. Connect your GitHub repo
2. Build settings: Leave blank (it's static HTML)
3. Deploy directory: `/`
4. Deploy!

### Your Own Server
Just upload all files via FTP/SSH to your web host.

## Customization

- **Colors:** Edit the `:root` variables in the `<style>` section
- **Logo:** Replace `your-logo.png` with your own (44×44px recommended)
- **Name:** Change "Your Site Name" in the header
- **Footer:** Update copyright and contact info

## Structure

Each post is a standalone HTML file. This means:
- ✅ Fast loading (no build step)
- ✅ Easy to edit (just open in VSCode)
- ✅ Works anywhere (pure HTML/CSS)
- ✅ Version controlled (see history in Git)

Happy blogging! 🚀