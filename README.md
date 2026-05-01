# AI/ML Developer Portfolio Website

A modern, responsive, and professional personal portfolio website built with vanilla HTML, CSS, and JavaScript. Perfect for Computer Science students specializing in AI/ML.

## 🚀 Features

- ✅ **Fully Responsive** - Works perfectly on mobile, tablet, and desktop
- ✅ **Dark Mode Toggle** - Persistent dark/light theme switcher
- ✅ **Smooth Scrolling Navigation** - Sticky navbar with smooth section navigation
- ✅ **Modern Design** - Clean, minimal, and professional UI with animations
- ✅ **SEO Optimized** - Meta tags and semantic HTML
- ✅ **Contact Form** - Email contact form with validation
- ✅ **Accessibility** - WCAG compliant with proper ARIA labels
- ✅ **No Framework Dependencies** - Pure vanilla HTML, CSS, and JavaScript

## 📁 Project Structure

```
portfolio/
├── index.html      # Main HTML file
├── styles.css      # All styling and responsive design
├── script.js       # JavaScript for interactivity
└── README.md       # This file
```

## 🔧 Setup & Customization

### 1. **Update Personal Information**

In `index.html`, replace the following placeholders:

#### Name & Professional Summary
- Search for **"Your Name"** and replace with your actual name
- Update the professional summary in the hero section

#### Resume Link (Google Drive)
```html
<!-- Find this line and replace the link -->
<a href="REPLACE_WITH_GOOGLE_DRIVE_RESUME_LINK" target="_blank">
    📄 Resume
</a>
```

**How to get your Google Drive resume link:**
1. Upload your resume PDF to Google Drive
2. Right-click → Share
3. Set to "Anyone with the link" and copy the share link
4. Modify the URL: Change `open?id=FILE_ID` to `/uc?id=FILE_ID`
5. Or use: `https://drive.google.com/uc?export=download&id=FILE_ID`

#### Essay PDF Link
```html
<!-- Find this line in the Essay section -->
<a href="REPLACE_WITH_GOOGLE_DRIVE_PDF_LINK" target="_blank">
    📄 View Full Essay (PDF)
</a>
```

#### Video Embed Link (Google Drive)
```html
<!-- Find this line in the Career Introduction section -->
<iframe
    src="REPLACE_WITH_GOOGLE_DRIVE_VIDEO_EMBED_LINK"
    ...
></iframe>
```

**How to get your Google Drive video embed link:**
1. Upload your video to Google Drive
2. Right-click → Share → Set to "Anyone with the link"
3. Get the FILE_ID from the share link
4. Use: `https://drive.google.com/file/d/FILE_ID/preview`

#### Contact Information
- Email: Update `mailto:your.email@example.com`
- LinkedIn: Update the LinkedIn URL
- GitHub: Update the GitHub URL

### 2. **Update Project Information**

In the Projects section, customize the 3 project cards:
- Project title
- Description
- Technologies used
- GitHub and Demo links

### 3. **Update Skills**

Modify the skills sections to match your expertise:
- AI & Machine Learning
- Programming Languages
- Web Development
- Tools & Technologies
- Proficiency levels in the bars section

### 4. **Customize Colors (Optional)**

Edit the CSS variables in `styles.css`:

```css
:root {
    --primary: #6366f1;        /* Primary brand color */
    --secondary: #ec4899;       /* Secondary accent color */
    --background: #ffffff;      /* Background color */
    --text-primary: #1a202c;    /* Main text color */
    /* ... other variables */
}
```

### 5. **Add Your Photo**

Replace the placeholder icon in the About section with your photo:

```html
<div class="image-placeholder">
    <img src="your-photo.jpg" alt="Your Name" style="width:100%; height:100%; object-fit:cover;">
</div>
```

## 🎨 Design Features

### Responsive Breakpoints
- **Desktop**: 1200px and above
- **Tablet**: 768px to 1199px
- **Mobile**: Below 768px
- **Small Mobile**: Below 480px

### Color Scheme
- **Light Mode**: Clean whites and grays with indigo accents
- **Dark Mode**: Deep blues and grays for reduced eye strain

### Animations
- Fade-in animations on scroll
- Hover effects on cards and buttons
- Smooth transitions throughout
- Progress bar animations

## 📝 Contact Form

The contact form includes:
- **Validation**: Checks for required fields and valid email format
- **Client-side Feedback**: Shows success/error messages
- **Responsive Design**: Works on all screen sizes

**To integrate with your email service:**

Currently, the form shows a success message without sending. To actually send emails, integrate with:

1. **Formspree** (Easiest)
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

2. **EmailJS**
   - Add EmailJS library
   - Configure with your service ID

3. **Your Backend API**
   - Replace the fetch call in `script.js` with your API endpoint

## 🌐 Deployment

### Option 1: GitHub Pages (Free)
1. Push to GitHub
2. Go to repository settings
3. Enable GitHub Pages from main branch
4. Your site will be live at `username.github.io/portfolio`

### Option 2: Netlify (Free & Easy)
1. Connect your GitHub repo to Netlify
2. Deploy automatically on push
3. Get a custom domain

### Option 3: Vercel (Free)
1. Import your GitHub repo
2. Deploy with one click
3. Get automatic SSL and optimization

## 🔍 SEO Optimization

The site includes:
- Meta tags for search engines
- Semantic HTML structure
- Open Graph tags for social sharing
- Mobile-friendly responsive design
- Fast loading times (no dependencies)

**To improve SEO further:**
1. Add descriptions to project cards
2. Include high-quality images
3. Create a sitemap.xml
4. Add schema.org structured data

## ♿ Accessibility

Features included:
- ARIA labels on interactive elements
- Semantic HTML tags
- Keyboard navigation support
- Color contrast compliance
- Reduced motion preferences respected

## 📱 Mobile Optimization

- Hamburger menu on mobile
- Touch-friendly buttons
- Responsive typography
- Optimized images
- Fast load times

## 🚀 Performance Tips

1. **Optimize Images**: Compress project images
2. **Lazy Loading**: Already implemented for images with `data-src`
3. **Minimize CSS/JS**: Combine files for production
4. **Use CDN**: Serve from edge locations
5. **Cache Headers**: Set proper cache headers

## 🐛 Troubleshooting

### Dark mode not persisting?
- Check browser's localStorage is enabled
- Try clearing browser cache

### Navigation links not working?
- Ensure section IDs match href values
- Check for JavaScript errors in console

### Forms not sending?
- Implement backend integration (see Contact Form section)
- Check browser console for errors

### Videos not embedding?
- Verify Google Drive video embed URL format
- Ensure video permissions are set to "Anyone with link"

## 📚 Resources

- [Google Drive Share Links](https://support.google.com/drive/answer/2881970)
- [Responsive Web Design](https://web.dev/responsive-web-design-basics/)
- [Web Accessibility](https://www.w3.org/WAI/fundamentals/)
- [CSS Variables](https://developer.mozilla.org/en-US/docs/Web/CSS/--*)

## 📄 License

This portfolio template is free to use and modify for personal or commercial projects.

## 💡 Tips for Success

1. **Keep it Updated**: Add new projects as you complete them
2. **Add Content Regularly**: Blog posts or articles about AI/ML
3. **Include Metrics**: Show project impact with data/statistics
4. **Professional Photo**: Use a high-quality headshot
5. **Proofread**: Check for typos and grammar
6. **Test on Devices**: Verify on real phones and tablets
7. **Share Portfolio**: Add link to LinkedIn, GitHub bio, resume

---

**Need Help?**
- Check the HTML comments in the code for specific sections
- Inspect elements in browser DevTools
- Test responsive design with device emulation

Happy coding! 🎉
