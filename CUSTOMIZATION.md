# Quick Customization Checklist

Use this checklist to quickly customize your personal website. Open the files mentioned and replace the placeholder text with your own information.

## 1. index.html - Personal Information

### Line 16: Navigation Brand
```html
<h1>Your Name</h1>
```
Replace "Your Name" with your actual name.

### Lines 32-38: Hero Section
```html
<h2 class="hero-title">Hi, I'm <span class="highlight">Your Name</span></h2>
<p class="hero-subtitle">Web Developer | Designer | Problem Solver</p>
<p class="hero-description">
    I create beautiful and functional websites that make a difference.
</p>
```
- Replace "Your Name" (appears in 2 places)
- Update job titles/roles in the subtitle
- Write your own tagline in the description

### Lines 50-75: About Me Section
```html
<p>
    I'm a passionate developer with a love for creating elegant solutions to complex problems.
    With a background in [Your Field], I've spent the last [X] years honing my skills in
    web development, design, and problem-solving.
</p>
```
- Replace [Your Field] with your background
- Replace [X] with your years of experience
- Update hobbies/interests in the second paragraph
- Modify statistics (years, projects, clients)

### Lines 90-125: Skills Section
Update the 4 skill cards with your actual skills:
- Skill icons (emojis or icon libraries)
- Skill titles
- Technologies/tools you know

### Lines 130-210: Projects Section
For each of the 3 projects:
- Project title
- Project description
- Technology tags
- Demo link (or remove if no demo)
- Source code link (GitHub repo)

### Lines 220-240: Contact Section
```html
<a href="mailto:your.email@example.com">your.email@example.com</a>
<a href="tel:+1234567890">+1 (234) 567-890</a>
<span>Your City, Country</span>
```
- Replace email address
- Update phone number
- Change location

### Lines 245-255: Social Media Links
```html
<a href="https://github.com/yourusername" target="_blank">
<a href="https://linkedin.com/in/yourusername" target="_blank">
<a href="https://twitter.com/yourusername" target="_blank">
```
Replace "yourusername" with your actual usernames.

### Line 295: Footer
```html
<p>&copy; 2024 Your Name. All rights reserved.</p>
```
Replace "Your Name" with your actual name.

## 2. styles.css - Colors & Design

### Lines 8-18: Color Variables
```css
:root {
    --primary-color: #4a90e2;      /* Main brand color */
    --secondary-color: #50c878;    /* Accent color */
    --accent-color: #f39c12;       /* Highlight color */
}
```
Change these hex color codes to match your personal brand.

### Line 117: Hero Background Gradient
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```
Customize the gradient colors to your preference.

## 3. assets/ - Images

Add these images to the `assets/` folder:

### Required:
- **profile.jpg** - Your profile picture (500x500px, square)
- **project1.jpg** - Screenshot of your first project (800x600px)
- **project2.jpg** - Screenshot of your second project (800x600px)
- **project3.jpg** - Screenshot of your third project (800x600px)

### Optional:
- **favicon.ico** - Browser tab icon (16x16 or 32x32px)
- Add to HTML: `<link rel="icon" href="assets/favicon.ico">`

## 4. Meta Tags & SEO

### Lines 4-6 in index.html:
```html
<meta name="description" content="Personal website - About Me">
<meta name="author" content="Your Name">
<title>About Me - Personal Website</title>
```
Update these for better SEO.

## 5. Contact Form Setup

Choose one option:

### Option A: Formspree (Easiest)
1. Sign up at https://formspree.io/
2. Create a form and get your form ID
3. Update line 265 in index.html:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST" id="contactForm">
```

### Option B: Keep JavaScript Alert
The form currently shows an alert. No changes needed if this is acceptable.

### Option C: Custom Backend
Update the commented code in script.js (lines 95-110) with your API endpoint.

## Quick Test Checklist

After customization:
- [ ] All "Your Name" replaced with actual name
- [ ] All links updated (email, phone, social media)
- [ ] All project links point to actual demos/repos
- [ ] Profile image added to assets folder
- [ ] Project images added to assets folder
- [ ] Colors match your personal brand
- [ ] Test on mobile device or browser dev tools
- [ ] All links work (click each one)
- [ ] Contact form works (test submission)

## Deploy

1. **GitHub Pages**: Push to GitHub → Settings → Pages → Enable
2. **Netlify**: Drag and drop project folder at https://app.netlify.com/drop
3. **Vercel**: Import from GitHub at https://vercel.com/

---

That's it! Your personal website is ready to go live! 🚀
