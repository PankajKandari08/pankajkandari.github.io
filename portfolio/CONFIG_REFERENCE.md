# Configuration Reference

This file contains all the exact replacements needed to customize your portfolio.

## 📝 REPLACEMENTS NEEDED

### 1. Personal Name Replacements

**Location:** `index.html`

Find and replace all instances of `Your Name`:

```html
<!-- Hero Section (Line ~65) -->
<h1 class="hero-title">Hi, I'm <span class="highlight">Your Name</span></h1>

<!-- About Section (Line ~95) -->
<h3 class="section-subtitle">Your Name</h3>

<!-- Footer (Line ~320) -->
<p>&copy; 2024 Your Name. All rights reserved.</p>

<!-- Title Tag (Line ~6) -->
<title>Your Name - AI/ML Developer Portfolio</title>
```

**Replace All:** `Your Name` → `Your Actual Name`

---

### 2. Resume Link

**Location:** `index.html`, Line ~62

```html
<!-- BEFORE -->
<a href="REPLACE_WITH_GOOGLE_DRIVE_RESUME_LINK" target="_blank" class="btn btn-primary btn-sm">
    📄 Resume
</a>

<!-- AFTER -->
<a href="https://drive.google.com/uc?export=download&id=YOUR_FILE_ID_HERE" target="_blank" class="btn btn-primary btn-sm">
    📄 Resume
</a>
```

**How to get the FILE_ID:**
1. Upload resume to Google Drive
2. Right-click → Share → Change to "Anyone with the link"
3. Copy link: `https://drive.google.com/file/d/FILE_ID/view?usp=sharing`
4. Extract the FILE_ID (between `/d/` and `/view`)

---

### 3. Essay PDF Link

**Location:** `index.html`, Line ~148

```html
<!-- BEFORE -->
<a href="REPLACE_WITH_GOOGLE_DRIVE_PDF_LINK" target="_blank" class="btn btn-primary">
    📄 View Full Essay (PDF)
</a>

<!-- AFTER -->
<a href="https://drive.google.com/file/d/YOUR_FILE_ID_HERE/preview" target="_blank" class="btn btn-primary">
    📄 View Full Essay (PDF)
</a>
```

**How to get the FILE_ID:**
1. Upload PDF to Google Drive
2. Right-click → Share → Change to "Anyone with the link"
3. Copy link and extract FILE_ID (same as above)

---

### 4. Career Video Embed Link

**Location:** `index.html`, Line ~161-170

```html
<!-- BEFORE -->
<iframe
    width="100%"
    height="500"
    src="REPLACE_WITH_GOOGLE_DRIVE_VIDEO_EMBED_LINK"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen>
</iframe>

<!-- AFTER -->
<iframe
    width="100%"
    height="500"
    src="https://drive.google.com/file/d/YOUR_FILE_ID_HERE/preview"
    frameborder="0"
    allow="autoplay; encrypted-media"
    allowfullscreen>
</iframe>
```

---

### 5. Contact Information

**Location:** `index.html`, Line ~282-295

```html
<!-- Email -->
<a href="mailto:your.email@example.com">your.email@example.com</a>

<!-- LinkedIn -->
<a href="https://linkedin.com/in/your-profile" target="_blank">linkedin.com/in/your-profile</a>

<!-- GitHub -->
<a href="https://github.com/your-username" target="_blank">github.com/your-username</a>
```

---

### 6. Professional Summary

**Location:** `index.html`, Line ~76-80

```html
<!-- BEFORE -->
<p class="hero-description">
    I'm passionate about building intelligent systems and exploring the intersection of
    AI/ML with real-world applications. With expertise in Python, Java, and web technologies,
    I'm committed to creating impactful solutions.
</p>

<!-- AFTER -->
Write your own 2-4 line professional summary highlighting:
- Your main interests (AI/ML, specific areas)
- Your key skills
- Your career goals
```

---

### 7. About Section Content

**Location:** `index.html`, Line ~94-106

```html
<!-- Update the about paragraphs with your background -->

<!-- First paragraph - Background -->
<p class="about-intro">
    I'm a Computer Science student with a passion for...
</p>

<!-- Following paragraphs - Your story, interests, and goals -->
<p>
    My journey in tech started with...
</p>
```

---

### 8. Essay Title and Description

**Location:** `index.html`, Line ~136-146

```html
<h3 class="essay-title">AI in Healthcare</h3>
<!-- Keep as is OR change if you have a different essay -->

<p class="essay-preview">
    Explore the transformative impact of Artificial Intelligence in modern healthcare.
    <!-- Update with your essay description -->
</p>

<!-- Update the tags to match your essay -->
<span class="tag">AI</span>
<span class="tag">Healthcare</span>
<span class="tag">Machine Learning</span>
```

---

### 9. Project Cards

**Location:** `index.html`, Line ~190-280 (3 project cards)

```html
<!-- Project 1 -->
<div class="project-card">
    <div class="project-image">
        <div class="image-placeholder-project">🤖</div>  <!-- Change emoji -->
    </div>
    <div class="project-content">
        <h3 class="project-title">ML Model for Sentiment Analysis</h3>  <!-- Your project title -->
        <p class="project-description">
            Built a machine learning model using TensorFlow and NLP techniques...
            <!-- Your project description -->
        </p>
        <div class="project-tech">
            <span class="tech-tag">Python</span>   <!-- Your tech stack -->
            <span class="tech-tag">TensorFlow</span>
            <!-- Add/remove tech tags -->
        </div>
        <div class="project-links">
            <a href="#" class="link-btn">GitHub</a>  <!-- Your GitHub link -->
            <a href="#" class="link-btn">Demo</a>    <!-- Your demo link -->
        </div>
    </div>
</div>
```

**Repeat for Project 2 and Project 3** (or add more cards as needed)

---

### 10. Skills - AI & Machine Learning

**Location:** `index.html`, Line ~296-303

```html
<div class="skill-category">
    <h3 class="skill-category-title">🤖 AI & Machine Learning</h3>
    <div class="skill-tags">
        <span class="skill-tag">Python</span>
        <span class="skill-tag">TensorFlow</span>
        <!-- Add your skills here -->
    </div>
</div>
```

**Repeat for:**
- Programming Languages
- Web Development
- Tools & Technologies

---

### 11. Proficiency Levels

**Location:** `index.html`, Line ~340-362

```html
<div class="proficiency-item">
    <label>Python</label>
    <div class="progress-bar">
        <div class="progress" style="width: 95%"></div>  <!-- 0-100% -->
    </div>
</div>
```

- Update labels to your skills
- Adjust width percentage based on proficiency
- Add or remove items as needed

---

### 12. About Section Image

**Location:** `index.html`, Line ~110-115

```html
<!-- BEFORE (Placeholder) -->
<div class="image-placeholder">
    <span class="placeholder-icon">👤</span>
</div>

<!-- AFTER (Your Photo) -->
<div class="image-placeholder">
    <img src="your-photo.jpg" alt="Your Name" style="width:100%; height:100%; object-fit:cover;">
</div>
```

---

## 🎨 Color Customization

**Location:** `styles.css`, Line ~15-27

```css
:root {
    --primary: #6366f1;        /* Main brand color - Change this */
    --primary-hover: #4f46e5;  /* Darker shade for hover */
    --secondary: #ec4899;       /* Accent color - Change this */
    --secondary-hover: #db2777; /* Darker accent */
    /* Keep others or customize */
}
```

**Example Color Schemes:**

Blue + Purple Theme:
```css
--primary: #3b82f6;        /* Blue */
--primary-hover: #2563eb;
--secondary: #8b5cf6;      /* Purple */
--secondary-hover: #7c3aed;
```

Green + Teal Theme:
```css
--primary: #10b981;        /* Green */
--primary-hover: #059669;
--secondary: #06b6d4;      /* Teal */
--secondary-hover: #0891b2;
```

---

## 📝 Content Update Checklist

- [ ] Update all instances of "Your Name"
- [ ] Update professional summary (hero section)
- [ ] Update about section content (background, interests, goals)
- [ ] Add resume link
- [ ] Add essay PDF link
- [ ] Add career video link
- [ ] Update email address
- [ ] Update LinkedIn URL
- [ ] Update GitHub URL
- [ ] Update 2-3 projects with descriptions and links
- [ ] Update AI/ML skills
- [ ] Update programming languages
- [ ] Update web development skills
- [ ] Update tools & technologies
- [ ] Update proficiency levels
- [ ] Add your photo
- [ ] Test all links and forms
- [ ] Test on mobile, tablet, and desktop
- [ ] Deploy to web

---

## 🔍 Finding and Replacing

### Using VS Code (Recommended)
1. Press `Ctrl+H` (or `Cmd+Shift+H` on Mac)
2. Type the text to find: `REPLACE_WITH_GOOGLE_DRIVE_RESUME_LINK`
3. Type the replacement: `https://drive.google.com/uc?export=download&id=YOUR_FILE_ID`
4. Click "Replace All"

### Using Other Editors
- Most text editors have Find & Replace (usually `Ctrl+H` or `Ctrl+Shift+H`)
- Open the feature and follow the same process

---

## ✅ Verification Checklist

After making all replacements:

- [ ] No placeholder text remains (REPLACE_WITH_...)
- [ ] All links are valid (test them!)
- [ ] Images load correctly
- [ ] Contact form works
- [ ] Mobile menu functions
- [ ] Dark mode toggles
- [ ] All sections scroll properly
- [ ] Resume downloads correctly
- [ ] Essay PDF opens
- [ ] Video plays
- [ ] No console errors (check DevTools)

---

## 🆘 Troubleshooting

### Links not working?
- Verify the full URL is correct
- Check for typos in FILE_ID
- Test the link in a new browser tab

### Images not showing?
- Verify image file is in same directory
- Check file name matches exactly (case-sensitive)
- Use absolute URLs if needed

### Form not working?
- Currently shows success message
- To actually send emails, integrate Formspree or EmailJS
- See SETUP_GUIDE.md for integration steps

### Video not playing?
- Verify video is uploaded to Google Drive
- Check sharing permissions (must be "Anyone with link")
- Use correct embed URL format

---

## 📞 Need Help?

Refer to:
1. `README.md` - Full documentation
2. `SETUP_GUIDE.md` - Step-by-step customization
3. Code comments in `index.html`, `styles.css`, `script.js`
4. Browser DevTools (F12) to debug issues

Good luck! 🚀
