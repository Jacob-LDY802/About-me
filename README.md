# Personal Website - About Me

A beautiful, responsive personal website to showcase your skills, projects, and personality. Easy to customize and deploy!

![Website Preview](assets/preview.jpg)

## 🌟 Features

- **Fully Responsive**: Works perfectly on desktop, tablet, and mobile devices
- **Modern Design**: Clean, professional layout with smooth animations
- **Easy to Customize**: Simple HTML/CSS/JavaScript structure
- **SEO Friendly**: Proper meta tags and semantic HTML
- **Fast Loading**: Optimized performance with minimal dependencies
- **Smooth Scrolling**: Enhanced user experience with scroll animations
- **Contact Form**: Built-in contact form (ready to connect to a backend)
- **Social Media Links**: Connect to your GitHub, LinkedIn, Twitter, and more

## 📁 Project Structure

```
About-me/
├── index.html          # Main HTML file
├── styles.css          # All styling
├── script.js           # JavaScript functionality
├── assets/             # Images and media files
│   ├── profile.jpg     # Your profile picture
│   ├── project1.jpg    # Project screenshots
│   ├── project2.jpg
│   └── project3.jpg
└── README.md           # This file
```

## 🚀 Quick Start

1. **Clone or Download** this repository
2. **Customize the content** (see customization guide below)
3. **Add your images** to the `assets/` folder
4. **Open `index.html`** in your browser to preview
5. **Deploy** to GitHub Pages, Netlify, or any static hosting service

## ✏️ Customization Guide

### 1. Personal Information

Open `index.html` and update the following sections:

#### Navigation & Hero Section (Lines 15-45)
```html
<!-- Change your name -->
<h1>Your Name</h1>

<!-- Update hero title and description -->
<h2 class="hero-title">Hi, I'm <span class="highlight">Your Name</span></h2>
<p class="hero-subtitle">Web Developer | Designer | Problem Solver</p>
<p class="hero-description">Your personal tagline here</p>
```

#### About Section (Lines 50-85)
- Replace `assets/profile.jpg` with your profile picture
- Update the text about yourself
- Modify the statistics (years of experience, projects, clients)

#### Skills Section (Lines 90-120)
- Add or remove skill cards
- Update skill icons (using emojis or icon libraries)
- Modify skill descriptions

#### Projects Section (Lines 125-200)
- Add your project titles and descriptions
- Update project images in the `assets/` folder
- Add your project demo and GitHub links
- Modify technology tags

#### Contact Section (Lines 205-250)
- Update your email address
- Change phone number
- Add your location
- Update social media links (GitHub, LinkedIn, Twitter)

### 2. Colors & Styling

Open `styles.css` and modify the CSS variables at the top:

```css
:root {
    --primary-color: #4a90e2;      /* Main brand color */
    --secondary-color: #50c878;    /* Accent color */
    --accent-color: #f39c12;       /* Highlight color */
    --text-primary: #333333;       /* Main text color */
    --text-secondary: #666666;     /* Secondary text */
    /* ... more variables */
}
```

### 3. Images

Add your images to the `assets/` folder:

- **profile.jpg**: Your profile picture (square, at least 500x500px recommended)
- **project1.jpg, project2.jpg, project3.jpg**: Screenshots of your projects (landscape orientation, 800x600px recommended)

> **Note**: The website includes fallback placeholder images, so it will work even without custom images.

### 4. Fonts

To change fonts, update the `--font-primary` variable in `styles.css`:

```css
--font-primary: 'Your Font Name', sans-serif;
```

Don't forget to import the font in the `<head>` of `index.html`:

```html
<link href="https://fonts.googleapis.com/css2?family=Your+Font+Name:wght@400;600;700&display=swap" rel="stylesheet">
```

### 5. Contact Form

The contact form currently shows an alert on submission. To make it functional:

#### Option A: Use Formspree (Easy, Free)
1. Sign up at [Formspree.io](https://formspree.io/)
2. Update the form action in `index.html`:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

#### Option B: Use EmailJS
1. Sign up at [EmailJS.com](https://www.emailjs.com/)
2. Follow their integration guide
3. Update the form handler in `script.js`

#### Option C: Connect to Your Backend
Update the commented code in `script.js` (lines 95-110) with your API endpoint.

## 🌐 Deployment

### GitHub Pages (Recommended)

1. Push your code to a GitHub repository
2. Go to repository Settings → Pages
3. Select your branch (usually `main`) and root folder
4. Your site will be live at `https://yourusername.github.io/repository-name/`

### Netlify

1. Sign up at [Netlify.com](https://www.netlify.com/)
2. Drag and drop your project folder
3. Your site is live instantly!

### Vercel

1. Sign up at [Vercel.com](https://vercel.com/)
2. Import your GitHub repository
3. Deploy with one click

### Custom Domain

Once deployed, you can connect a custom domain through your hosting provider's settings.

## 🎨 Customization Tips

### Adding More Sections

To add a new section, follow this pattern in `index.html`:

```html
<section id="new-section" class="new-section">
    <div class="container">
        <h2 class="section-title">Section Title</h2>
        <!-- Your content here -->
    </div>
</section>
```

Add the navigation link:
```html
<li><a href="#new-section">New Section</a></li>
```

### Changing Layout

The website uses CSS Grid for layouts. To adjust:
- Grid columns: Modify `grid-template-columns` in relevant sections
- Spacing: Change `gap` values
- Responsive breakpoints: Edit `@media` queries at the bottom of `styles.css`

### Adding Animations

The website includes scroll animations via Intersection Observer. To add more:

```javascript
const newElements = document.querySelectorAll('.your-class');
newElements.forEach(element => {
    observer.observe(element);
});
```

## 📱 Mobile Optimization

The website is fully responsive with breakpoints at:
- 768px (tablet)
- 480px (mobile)

Test your site on different devices using browser dev tools.

## 🛠️ Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Feel free to fork this project and customize it for your own use. If you create something cool, share it!

## 💡 Tips for Success

1. **Keep it Updated**: Regularly update your projects and achievements
2. **Professional Photos**: Use high-quality, professional images
3. **Concise Content**: Keep descriptions brief and impactful
4. **Test Everything**: Check all links and ensure contact form works
5. **SEO**: Update meta tags for better search engine visibility
6. **Performance**: Optimize images (use WebP format when possible)
7. **Accessibility**: Ensure proper alt tags and ARIA labels

## 📞 Need Help?

If you have questions or run into issues:
1. Check the browser console for errors
2. Validate your HTML/CSS
3. Make sure all file paths are correct
4. Test in different browsers

## 🎯 What's Next?

Consider adding:
- Blog section
- Testimonials
- Resume/CV download
- Dark mode toggle
- More interactive elements
- Analytics (Google Analytics)
- Live chat widget

---

**Made with ❤️ and lots of ☕**

Good luck with your personal website! Remember to make it uniquely yours! 🚀
