# Kuldeep Verma - Portfolio Website 🚀

A stunning, interactive portfolio website built with modern web technologies, featuring 3D animations, particle systems, and responsive design.

## ✨ Features

- **Interactive 3D Animations**: Card tilt effects, floating elements, and smooth transitions
- **Particle System**: Dynamic background particles with mouse interaction
- **Responsive Design**: Optimized for all devices (mobile, tablet, desktop)
- **Smooth Scrolling**: Seamless navigation between sections
- **Contact Form**: Direct email integration using mailto
- **Dark Theme**: Modern dark color scheme with gradient accents
- **Performance Optimized**: Lazy loading, intersection observers, and smooth animations
- **Easter Eggs**: Hidden Konami code activation
- **Cursor Trail**: Interactive cursor following effect (desktop only)

## 🛠 Technologies Used

- **HTML5**: Semantic markup and modern structure
- **CSS3**: Advanced animations, gradients, and responsive design
- **Vanilla JavaScript**: Interactive features and animations
- **Font Awesome**: Beautiful icons
- **Google Fonts**: Poppins font family

## 📁 File Structure

```
portfolio/
├── index.html          # Main HTML file
├── style.css           # CSS styles and animations
├── script.js           # JavaScript functionality
├── README.md           # This file
└── assets/             # (Optional) Images and other assets
    └── profile-photo.jpg  # Your profile photo
```

## 🚀 Quick Start

### 1. Clone or Download the Files

Create a new folder for your portfolio and add these files:

1. **index.html** - The main HTML structure
2. **style.css** - All styling and animations
3. **script.js** - Interactive functionality
4. **Your profile photo** (optional - currently uses placeholder)

### 2. Customize Your Content

#### Update Personal Information in `index.html`:

```html
<!-- Update these sections with your information -->
<h1>Hi, I'm <span class="gradient-text">Your Name</span></h1>
<p class="hero-subtitle">Your Title/Role</p>

<!-- Update contact information -->
<a href="mailto:your-email@gmail.com">your-email@gmail.com</a>
<a href="tel:+1234567890">+1 234-567-890</a>

<!-- Update social links -->
<a href="https://linkedin.com/in/your-profile" target="_blank">
<a href="https://github.com/your-username" target="_blank">
```

#### Add Your Profile Photo:

Replace the placeholder image in the hero section:

```html
<img src="your-profile-photo.jpg" alt="Your Name" class="profile-img">
```

#### Update Projects:

Modify the projects section with your actual projects:

```html
<div class="project-card">
    <div class="project-icon">
        <i class="fas fa-your-icon"></i>
    </div>
    <h3>Your Project Name</h3>
    <p>Your project description...</p>
    <div class="project-tech">
        <span class="tech-tag">Technology 1</span>
        <span class="tech-tag">Technology 2</span>
    </div>
</div>
```

### 3. Local Development

Simply open `index.html` in your web browser to view the website locally.

For better development experience, you can use a local server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js (with http-server)
npx http-server

# Using PHP
php -S localhost:8000
```

## 🌐 Deploy to Vercel

### Method 1: GitHub Repository (Recommended)

1. **Create a GitHub Repository**:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio setup"
   git branch -M main
   git remote add origin https://github.com/yourusername/your-portfolio.git
   git push -u origin main
   ```

2. **Deploy on Vercel**:
   - Go to [vercel.com](https://vercel.com)
   - Sign up/login with GitHub
   - Click "New Project"
   - Import your GitHub repository
   - Click "Deploy"

### Method 2: Direct Upload

1. **Prepare Files**:
   - Ensure all files are in the root directory
   - Make sure `index.html` is in the root

2. **Deploy**:
   - Go to [vercel.com](https://vercel.com)
   - Drag and drop your project folder
   - Vercel will automatically deploy

### Method 3: Vercel CLI

1. **Install Vercel CLI**:
   ```bash
   npm i -g vercel
   ```

2. **Deploy**:
   ```bash
   vercel
   ```

## ⚙️ Configuration

### Email Integration

The contact form uses `mailto:` to open the user's default email client. Update the email address in both:

1. **HTML** (multiple locations):
   ```html
   <a href="mailto:your-email@gmail.com">your-email@gmail.com</a>
   ```

2. **JavaScript** (script.js):
   ```javascript
   const mailtoLink = `mailto:your-email@gmail.com?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(\`Name: ${name}\\nEmail: ${email}\\n\\nMessage:\\n${message}\`)}`;
   ```

### Customizing Colors

Update CSS variables in `style.css`:

```css
:root {
    --primary-color: #6366f1;      /* Main brand color */
    --secondary-color: #8b5cf6;    /* Secondary brand color */
    --accent-color: #06b6d4;       /* Accent color */
    /* ... other variables */
}
```

### Adding Your Resume

1. Add a resume file to your project (e.g., `resume.pdf`)
2. Add a download button in the hero section:

```html
<a href="resume.pdf" download class="btn btn-secondary">
    <i class="fas fa-download"></i> Download Resume
</a>
```

## 📱 Responsive Breakpoints

- **Desktop**: 1200px and above
- **Tablet**: 768px - 1199px
- **Mobile**: Below 768px
- **Small Mobile**: Below 480px

## 🎨 Customization Tips

### Adding New Sections

1. Add HTML structure:
```html
<section id="new-section" class="new-section">
    <div class="container">
        <h2 class="section-title">New Section</h2>
        <!-- Your content here -->
    </div>
</section>
```

2. Add navigation link:
```html
<li><a href="#new-section" class="nav-link">New Section</a></li>
```

3. Add CSS styles following the existing pattern

### Modifying Animations

All animations are defined in CSS. Key animation classes:

- `.fadeInUp` - Fade in from bottom
- `.slideInLeft` - Slide in from left
- `.slideInRight` - Slide in from right
- `.float` - Floating animation

## 🔧 Troubleshooting

### Common Issues:

1. **Animations not working**: Check if JavaScript is enabled
2. **Form not working**: Ensure email client is configured
3. **Responsive issues**: Test CSS media queries
4. **Performance issues**: Check image sizes and optimization

### Performance Optimization:

1. **Optimize Images**:
   - Use WebP format for better compression
   - Compress images before uploading
   - Use appropriate sizes for different devices

2. **Minimize Files**:
   - Minify CSS and JavaScript for production
   - Remove unused code

## 📊 SEO Optimization

Add these meta tags to improve SEO:

```html
<head>
    <!-- Existing meta tags -->
    <meta name="description" content="Kuldeep Verma - AI/ML Engineer specializing in Generative AI, LLM fine-tuning, and RAG systems">
    <meta name="keywords" content="AI, ML, Python, Generative AI, LLM, Portfolio">
    <meta name="author" content="Kuldeep Verma">
    
    <!-- Open Graph -->
    <meta property="og:title" content="Kuldeep Verma - AI/ML Engineer">
    <meta property="og:description" content="Portfolio showcasing AI/ML projects and expertise">
    <meta property="og:image" content="your-profile-photo.jpg">
    <meta property="og:url" content="https://your-domain.vercel.app">
</head>
```

## 🚀 Advanced Features

### Adding Google Analytics

```html
<!-- Add before closing </head> tag -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_TRACKING_ID"></script>
<script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'GA_TRACKING_ID');
</script>
```

### Custom Domain Setup

1. Purchase a domain from any registrar
2. In Vercel dashboard, go to your project
3. Click "Settings" → "Domains"
4. Add your custom domain
5. Update DNS records as instructed

## 📞 Support

If you need help with customization or have questions:

1. Check the code comments for guidance
2. Refer to the documentation links provided
3. Test changes locally before deploying

## 🎯 Next Steps

After deployment, consider:

1. **Analytics Setup**: Track visitors and engagement
2. **Blog Integration**: Add a blog section for content
3. **CMS Integration**: Use headless CMS for easy updates
4. **PWA Features**: Make it a Progressive Web App
5. **Advanced Animations**: Add more interactive elements

---

**Built with ❤️ by Kuldeep Verma**

*Ready to showcase your AI/ML expertise to the world! 🌟*"# KD_Protfoliyo" 
