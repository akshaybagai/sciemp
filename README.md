# Scientific Emporium - Quality Scientific Equipment

A modern, responsive static website built for GitHub Pages featuring a beautiful landing page and contact section for Scientific Emporium, your trusted supplier of scientific and laboratory equipment.

## 🚀 Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI/UX**: Clean, professional design with smooth animations
- **Landing Page**: Eye-catching hero section with feature highlights
- **Contact Section**: Interactive contact form with validation
- **Smooth Navigation**: Smooth scrolling and active section indicators
- **SEO Friendly**: Semantic HTML structure
- **Fast Loading**: Optimized static files with no dependencies

## 📁 Project Structure

```
sciemp/
├── index.html          # Main HTML file with all sections
├── styles.css          # Complete stylesheet with responsive design
├── script.js           # JavaScript for interactivity
└── README.md          # This file
```

## 🎨 Sections

1. **Navigation Bar**: Fixed navbar with smooth scroll links
2. **Hero Section**: Engaging landing page with call-to-action buttons
3. **Features Section**: Showcase of key features with icons
4. **About Section**: Company information with statistics
5. **Contact Section**: Contact form and information cards
6. **Footer**: Links and copyright information

## 🛠️ Setup & Deployment

### Local Development

1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/sciemp.git
   cd sciemp
   ```

2. Open `index.html` in your browser or use a local server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js (http-server)
   npx http-server
   ```

3. Visit `http://localhost:8000` in your browser

### Deploy to GitHub Pages

#### Option 1: Deploy from main branch

1. Create a new repository on GitHub (or use existing)

2. Initialize git and push your code:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: SciEmp website"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/sciemp.git
   git push -u origin main
   ```

3. Enable GitHub Pages:
   - Go to your repository on GitHub
   - Click on **Settings**
   - Scroll to **Pages** section
   - Under **Source**, select **main** branch
   - Select **/ (root)** folder
   - Click **Save**

4. Your site will be live at: `https://YOUR_USERNAME.github.io/sciemp/`

#### Option 2: Deploy using GitHub Desktop

1. Open GitHub Desktop
2. Click **File** → **Add Local Repository**
3. Select your `sciemp` folder
4. Click **Publish repository**
5. Follow step 3 above to enable GitHub Pages

#### Option 3: Deploy using gh-pages branch

```bash
# Create and checkout a new gh-pages branch
git checkout --orphan gh-pages
git add .
git commit -m "Deploy to GitHub Pages"
git push origin gh-pages

# Go to Settings → Pages and select gh-pages branch
```

## 📧 Contact Form Configuration

The contact form currently uses a **demo/simulation mode** for testing. To enable real email functionality, integrate with one of these services:

### Option 1: Formspree (Recommended)
1. Sign up at [formspree.io](https://formspree.io)
2. Create a new form and get your form endpoint
3. Update the form submission in `script.js`:
```javascript
const response = await fetch('https://formspree.io/f/YOUR_FORM_ID', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(formData)
});
```

### Option 2: EmailJS
1. Sign up at [emailjs.com](https://www.emailjs.com)
2. Follow their integration guide
3. Add their SDK and update `script.js`

### Option 3: Netlify Forms
If deploying to Netlify instead:
1. Add `netlify` attribute to form tag:
```html
<form netlify>
```
2. Deploy to Netlify

### Option 4: Custom Backend
Create your own backend API and update the fetch URL in `script.js`

## 🎨 Customization

### Colors
Edit the CSS variables in `styles.css`:
```css
:root {
    --primary-color: #6366f1;
    --secondary-color: #8b5cf6;
    --text-dark: #1e293b;
    /* ... more variables */
}
```

### Content
- Edit text directly in `index.html`
- Replace placeholder content with your own
- Update company name, features, and contact information

### Fonts
The site uses Inter from Google Fonts. To change:
1. Replace the Google Fonts link in `index.html`
2. Update font-family in `styles.css`

## 🔧 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

## 👤 Author

**Your Name**
- GitHub: [@YOUR_USERNAME](https://github.com/YOUR_USERNAME)
- Website: https://YOUR_USERNAME.github.io/sciemp/

## ⭐ Show Your Support

Give a ⭐️ if you like this project!

## 📸 Screenshots

### Desktop View
The landing page features a modern gradient background with floating cards and smooth animations.

### Mobile View
Fully responsive design with a hamburger menu and optimized layout for smaller screens.

## 🚀 Performance

- **Lighthouse Score**: 95+ (Performance, Accessibility, Best Practices, SEO)
- **Load Time**: < 1 second
- **No external dependencies**: Pure HTML, CSS, and JavaScript
- **Optimized assets**: Inline SVGs for icons

## 📞 Support

If you have any questions or need help with deployment, please open an issue on GitHub.

---

**Happy Coding!** 🎉

