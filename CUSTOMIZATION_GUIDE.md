# Robotics PhD Student Personal Website - Customization Guide

This website is built using Jekyll and the Academic Pages template, customized for a PhD student in Robotics.

## Website Structure

Your website includes the following main sections:

### 1. About Me (Homepage)
- **File:** `_pages/about.md`
- Contains your bio and research interests
- Customize with your personal information and research focus areas

### 2. Publications
- **Directory:** `_publications/`
- Each publication is a separate Markdown file
- Currently includes 5 sample robotics publications
- To add a new publication, create a new `.md` file with the following format:

```markdown
---
title: "Your Paper Title"
collection: publications
category: conferences  # or "manuscripts" for journal articles
permalink: /publication/YYYY-MM-DD-short-name
excerpt: 'Brief description of the paper'
date: YYYY-MM-DD
venue: 'Conference or Journal Name'
paperurl: # 'Link to paper PDF'
citation: 'Full citation format'
---

Additional details about the paper...
```

### 3. Education (CV)
- **File:** `_pages/cv.md`
- Contains education history, research experience, skills, and awards
- Update with your actual academic background and achievements

### 4. Awards
- **File:** `_pages/awards.md`
- Lists academic awards, scholarships, grants, and recognitions
- Add your own awards and honors

### 5. Contact
- **File:** `_pages/contact.md`
- Contact information and office details
- Update with your actual email, office location, and contact details

## Configuration

### Site-Wide Settings
Edit `_config.yml` to customize:

1. **Basic Information:**
   - `title`: Your name or site title
   - `name`: Your full name
   - `description`: Site description
   - `url`: Your GitHub Pages URL (https://YOUR-USERNAME.github.io)

2. **Author Profile (Sidebar):**
   ```yaml
   author:
     avatar: "profile.png"  # Your profile photo
     name: "Your Name"
     bio: "Your short bio"
     location: "Your University"
     employer: "Your Department"
     email: "your.email@university.edu"
     googlescholar: "Your Google Scholar URL"
     github: "your-github-username"
   ```

3. **Profile Photo:**
   - Place your profile photo in the `images/` directory
   - Name it `profile.png` or update the `avatar` field in `_config.yml`

### Navigation Menu
Edit `_data/navigation.yml` to customize the top menu:

```yaml
main:
  - title: "Publications"
    url: /publications/
  - title: "Education"
    url: /cv/
  - title: "Awards"
    url: /awards/
  - title: "Contact"
    url: /contact/
```

## How to Customize

### Step 1: Update Your Information
1. Edit `_config.yml` with your personal information
2. Replace placeholder text in all `_pages/*.md` files
3. Update email addresses, university names, and advisor names

### Step 2: Add Your Profile Photo
1. Prepare a professional square photo (recommended: 300x300px or larger)
2. Save it as `images/profile.png`
3. Or use a different filename and update `_config.yml` accordingly

### Step 3: Add Your Publications
1. Delete sample publications from `_publications/` directory
2. Create new `.md` files for each of your publications
3. Use the format shown above
4. Optional: Add PDF files to the `files/` directory and link to them

### Step 4: Update Your CV/Education
1. Edit `_pages/cv.md`
2. Add your actual degrees, research experience, and skills
3. Update the awards section

### Step 5: Customize Awards
1. Edit `_pages/awards.md`
2. Add your actual awards, honors, and recognitions

### Step 6: Update Contact Information
1. Edit `_pages/contact.md`
2. Add your real email, office location, and contact details

### Step 7: Add Social Media Links
In `_config.yml`, add your profiles:
```yaml
author:
  googlescholar: "https://scholar.google.com/citations?user=YOUR_ID"
  github: "your-github-username"
  linkedin: # Your LinkedIn username
  orcid: # Your ORCID URL
```

## Deployment

This website is automatically deployed to GitHub Pages when you push changes to the main branch.

### Testing Locally (Optional)
To test the site locally before deploying:

1. Install Ruby and Bundler
2. Run `bundle install` to install dependencies
3. Run `bundle exec jekyll serve` to start the local server
4. Visit `http://localhost:4000` in your browser

Alternatively, use Docker:
```bash
docker compose up
```

## File Organization

```
.
├── _config.yml              # Main configuration file
├── _data/
│   └── navigation.yml       # Top menu navigation
├── _pages/                  # Main pages
│   ├── about.md            # Homepage
│   ├── cv.md               # CV/Education page
│   ├── awards.md           # Awards page
│   └── contact.md          # Contact page
├── _publications/           # Publication entries
├── images/                  # Images and photos
│   └── profile.png         # Your profile photo
└── files/                   # PDF files and other documents
```

## Tips

1. **Keep it Professional:** Use a professional email and maintain academic tone
2. **Update Regularly:** Add new publications and awards as you earn them
3. **Link to PDFs:** Upload paper PDFs to `files/` directory and link them
4. **Use Google Scholar:** Link to your Google Scholar profile for citation metrics
5. **GitHub Repository:** Link to your GitHub for code and open-source projects

## Additional Resources

- [Academic Pages Documentation](https://academicpages.github.io/)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Markdown Guide](https://www.markdownguide.org/)

## Support

If you need help or encounter issues:
1. Check the [Academic Pages GitHub repository](https://github.com/academicpages/academicpages.github.io)
2. Read the [Jekyll documentation](https://jekyllrb.com/docs/)
3. Search for solutions in the GitHub issues

---

**Note:** Remember to replace all placeholder text with your actual information before making your site public!
