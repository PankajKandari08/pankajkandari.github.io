# Quick Setup Guide

## 📋 Pre-Requisites Checklist

Before customizing your portfolio, prepare the following:

- [ ] Your name and professional summary
- [ ] Resume PDF (uploaded to Google Drive)
- [ ] Essay PDF: "AI in Healthcare" (uploaded to Google Drive)
- [ ] Career introduction video (uploaded to Google Drive)
- [ ] Professional photo/headshot
- [ ] 2-3 project descriptions with tech stacks
- [ ] Email address for contact form
- [ ] LinkedIn profile URL
- [ ] GitHub profile URL

---

## 🚀 Step-by-Step Customization

### Step 1: Replace Your Name (5 mins)
1. Open `index.html` in your text editor
2. Find all instances of **"Your Name"** (use Find & Replace)
3. Replace with your actual name
4. Also update the footer copyright: `© 2024 Your Name`

### Step 2: Update Professional Summary (5 mins)
1. In the **Hero Section**, update:
   - `<h1>` - Your name and title
   - `.hero-subtitle` - Your professional tagline
   - `.hero-description` - 2-4 line professional summary

2. In the **About Section**, update:
   - `.about-intro` - Your background and education
   - Following paragraphs - Your interests and learning mindset

### Step 3: Add Google Drive Links (10 mins)

#### Resume Link
1. Open Google Drive
2. Upload your resume PDF
3. Right-click → Share → "Anyone with the link"
4. Copy the share link
5. Extract the FILE_ID (between `/d/` and `/`)
6. In `index.html`, find this line in navbar:
   ```html
   <a href="REPLACE_WITH_GOOGLE_DRIVE_RESUME_LINK" target="_blank">
   ```
7. Replace with: `https://drive.google.com/uc?export=download&id=YOUR_FILE_ID`

#### Essay PDF Link
1. Upload your essay PDF to Google Drive
2. Share with "Anyone with the link"
3. Extract FILE_ID
4. Find this line in **Essay Section**:
   ```html
   <a href="REPLACE_WITH_GOOGLE_DRIVE_PDF_LINK" target="_blank">
   ```
5. Replace with: `https://drive.google.com/file/d/YOUR_FILE_ID/preview`

#### Video Embed Link
1. Upload your video to Google Drive
2. Share with "Anyone with the link"
3. Extract FILE_ID
4. Find this line in **Career Introduction Section**:
   ```html
   <iframe src="REPLACE_WITH_GOOGLE_DRIVE_VIDEO_EMBED_LINK" ...>
   ```
5. Replace with: `https://drive.google.com/file/d/YOUR_FILE_ID/preview`

### Step 4: Update Contact Information (3 mins)
In the **Contact Section**, replace:
- `mailto:your.email@example.com` → Your actual email
- LinkedIn URL → Your LinkedIn profile
- GitHub URL → Your GitHub profile

### Step 5: Customize Projects (15 mins)
In the **Projects Section**, for each project card, update:
1. Project title
2. Project description
3. Technology tags (replace with your actual tech stack)
4. GitHub link (or remove if not public)
5. Demo link (or remove if not available)

### Step 6: Update Skills (10 mins)
In the **Skills Section**, customize:

1. **AI & Machine Learning** - Add your ML skills
2. **Programming Languages** - Your programming expertise
3. **Web Development** - Web tech you know
4. **Tools & Technologies** - Tools you use

Also update **Proficiency Levels**:
```html
<div class="proficiency-item">
    <label>Your Skill</label>
    <div class="progress-bar">
        <div class="progress" style="width: 85%"></div>
    </div>
</div>
```

Change the width percentage (0-100%) to reflect your proficiency.

### Step 7: Add Your Photo (5 mins)
In the **About Section**, replace the placeholder:
```html
<div class="image-placeholder">
    <span class="placeholder-icon">👤</span>
</div>
```

With:
```html
<div class="image-placeholder">
    <img src="your-photo.jpg" alt="Your Name" style="width:100%; height:100%; object-fit:cover;">
</div>
```

Place `your-photo.jpg` in the same folder as `index.html`.

---

## 🎨 (Optional) Customize Colors

Edit the CSS variables in `styles.css`:

```css
:root {
    --primary: #6366f1;        /* Change primary color (indigo) */
    --secondary: #ec4899;       /* Change accent color (pink) */
    /* ... other variables */
}
```

Popular color combinations:
- Blue + Purple: `#3b82f6` + `#8b5cf6`
- Green + Teal: `#10b981` + `#06b6d4`
- Orange + Red: `#f97316` + `#ef4444`

---

## 🧪 Testing Checklist

After customization, verify:

- [ ] All links work (navigation, buttons, external links)
- [ ] Mobile menu opens and closes
- [ ] Dark mode toggle works
- [ ] Responsive design on mobile, tablet, desktop
- [ ] Contact form validation works
- [ ] All content displays correctly
- [ ] Images load properly
- [ ] Video plays in Career section
- [ ] PDF opens when clicking essay button
- [ ] Resume downloads when clicking button

---

## 🚀 Deployment Options

### Deploy to GitHub Pages (Easiest)
1. Create a GitHub account
2. Create a new repository named `portfolio`
3. Push your files to GitHub
4. Go to Settings → Pages → Select "main" branch
5. Your site is now live at: `https://username.github.io/portfolio`

### Deploy to Netlify (Free)
1. Go to netlify.com
2. Click "New site from Git"
3. Connect your GitHub
4. Deploy automatically
5. Get free SSL and custom domain

### Deploy to Vercel (Free)
1. Go to vercel.com
2. Import your GitHub repo
3. One-click deployment
4. Get automatic optimization

---

## 📊 Recommended Content

### About Section
- Your background (education, years of experience)
- Why you're interested in AI/ML
- Key achievements or projects
- Learning mindset and continuous growth

### Projects Section
- 2-5 relevant projects minimum
- For each project include:
  - Clear title and description
  - Specific technologies used
  - Quantifiable results if possible (e.g., "92% accuracy", "50ms latency")
  - Links to GitHub repo or live demo

### Skills Section
- Group by category (AI/ML, Languages, Web Dev, Tools)
- Be honest about proficiency levels
- Include both soft and technical skills
- Update regularly as you learn new skills

---

## 🔗 Useful Links

- [Google Drive File Download Link Generator](https://www.embed-drive.com/)
- [Netlify Deployment Guide](https://docs.netlify.com/get-started/build-and-deploy/)
- [GitHub Pages Setup](https://pages.github.com/)
- [Color Palette Generator](https://coolors.co/)
- [Responsive Design Tester](https://responsivedesignchecker.com/)

---

## 💡 Pro Tips

1. **Keep Resume Updated**: Always have the latest version uploaded
2. **Regular Updates**: Add new projects quarterly
3. **Mobile First**: Test on your phone before deploying
4. **Professional Tone**: Use clear, concise language
5. **Showcase Impact**: Include metrics and results
6. **Call to Action**: Make it easy for recruiters to contact you
7. **SEO**: Update meta description in HTML for better search ranking
8. **Backup**: Keep git commits as you update your site

---

## ❓ Common Questions

### Q: Can I use my own domain?
**A:** Yes! Both Netlify and Vercel allow custom domains. See their documentation.

### Q: How do I add more projects?
**A:** Copy one project card in the HTML and paste it below. Update the content.

### Q: Can I change the design?
**A:** Yes! All styling is in `styles.css`. Modify colors, fonts, spacing as needed.

### Q: Is JavaScript required for deployment?
**A:** No, this is a static site. Just upload HTML, CSS, and JS to any hosting.

### Q: How do I track contact form submissions?
**A:** Integrate with Formspree, EmailJS, or your own backend API.

---

## 🎉 You're Ready!

Your portfolio is now ready to showcase your AI/ML skills and projects. 

**Next Steps:**
1. Customize with your information
2. Test on multiple devices
3. Deploy to web
4. Share your portfolio with recruiters and peers
5. Keep it updated with new projects and skills

Good luck! 🚀
