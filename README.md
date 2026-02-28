# PhD Portfolio Website

A sleek, minimalist single-page portfolio website designed for GitHub Pages, featuring a black theme with smooth navigation and responsive design.

## 🚀 Quick Start

1. **Clone or download** this repository
2. **Customize** the content (see instructions below)
3. **Deploy** to GitHub Pages (see deployment instructions below)

## 📝 Customization Guide

### 1. Update Personal Information

Open `index.html` and replace the placeholder content:

#### About Section
- **Your Photo**: Replace the image placeholder with your actual photo
  - Option A: Add an image file (e.g., `photo.jpg`) to the repository
  - Option B: In `index.html`, replace the `.image-placeholder` div content with:
    ```html
    <img src="photo.jpg" alt="Your Name" style="width: 300px; height: 300px; border-radius: 50%; object-fit: cover;">
    ```

- **Name and Title**: Update lines with "Your Name" and "PhD Candidate"
- **Bio**: Replace the placeholder paragraphs with your actual background and research interests
- **LinkedIn URL**: Update the `href` attribute in the LinkedIn button:
  ```html
  <a href="https://www.linkedin.com/in/your-actual-profile" ...>
  ```

#### Publications Section
For each publication, update:
- **Title**: Publication name
- **Authors**: Author list (your name is bolded with `<strong>`)
- **Venue**: Conference/Journal name and year
- **Abstract**: Brief description
- **Links**: Update `href` attributes with actual links to papers, code, etc.

Add or remove publication cards as needed by copying/deleting the `.publication-card` divs.

#### Projects Section
For each project, update:
- **Project Name**: Title of the project
- **Status**: Current/Ongoing/Completed/Past
- **Description**: Brief explanation of the project
- **Tags**: Replace with relevant technologies/methods
- **Link**: Update `href` with project links or GitHub repositories

Add or remove project cards by copying/deleting the `.project-card` divs.

#### Footer
Update the copyright year and name:
```html
<p>&copy; 2026 Your Actual Name. All rights reserved.</p>
```

### 2. Add Your Photo

Two methods to add your profile photo:

**Method 1: Using an image file**
1. Add your photo to the repository (e.g., `profile.jpg`)
2. In `index.html`, find the `.image-placeholder` div and replace it with:
```html
<img src="profile.jpg" alt="Your Name" class="profile-image" style="width: 300px; height: 300px; border-radius: 50%; object-fit: cover; border: 3px solid #333;">
```

**Method 2: Using CSS background image**
1. Add your photo to the repository
2. In `styles.css`, add this rule:
```css
.image-placeholder {
    background-image: url('profile.jpg');
    background-size: cover;
    background-position: center;
}
.image-placeholder p,
.image-placeholder span {
    display: none;
}
```

### 3. Customize Colors (Optional)

The default theme uses a black background with gray accents. To customize:

Open `styles.css` and modify the CSS custom properties at the top:

```css
:root {
    --color-bg: #0a0a0a;           /* Main background */
    --color-bg-alt: #1a1a1a;       /* Card backgrounds */
    --color-text: #cccccc;          /* Main text */
    --color-text-secondary: #999999; /* Secondary text */
    --color-accent: #333333;        /* Accent elements */
    --color-accent-hover: #444444;  /* Hover states */
    --color-border: #222222;        /* Borders */
}
```

## 🌐 Deployment to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and create a new repository
2. Name it `your-username.github.io` (for user site) or any name (for project site)
3. Make the repository **public**

### Step 2: Upload Files

**Option A: Using Git (Command Line)**
```bash
# Initialize git in your project folder
git init

# Add all files
git add .

# Commit the files
git commit -m "Initial commit: Portfolio website"

# Add your GitHub repository as remote
git remote add origin https://github.com/your-username/repository-name.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Option B: Using GitHub Web Interface**
1. Go to your repository on GitHub
2. Click "Add file" → "Upload files"
3. Drag and drop all your files (`index.html`, `styles.css`, `script.js`, and any images)
4. Click "Commit changes"

### Step 3: Enable GitHub Pages

1. Go to your repository settings
2. Scroll down to the "Pages" section (in the left sidebar)
3. Under "Source", select:
   - **Branch**: `main` (or `master`)
   - **Folder**: `/ (root)`
4. Click "Save"

### Step 4: Access Your Website

After a few minutes, your site will be live at:
- User site: `https://your-username.github.io`
- Project site: `https://your-username.github.io/repository-name`

GitHub will show you the URL in the Pages settings.

## 📱 Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Smooth Navigation**: Click navigation links to smoothly scroll to sections
- **Active Section Highlighting**: Navigation automatically highlights the current section
- **Mobile Menu**: Hamburger menu for mobile devices
- **Hover Effects**: Interactive elements with subtle animations
- **Dark Theme**: Professional black background with gray accents
- **SEO Ready**: Proper meta tags and semantic HTML structure

## 🛠️ Technical Details

### Browser Support
- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile browsers (iOS Safari, Chrome Mobile)

### Dependencies
- **None!** This is a pure HTML, CSS, and JavaScript website with no external frameworks or libraries

### File Structure
```
github_pages/
├── index.html          # Main HTML structure
├── styles.css          # All styling
├── script.js           # Navigation and interactions
├── README.md          # This file
└── [your-images]      # Your photos and assets
```

## 🎨 Customization Tips

### Adding More Sections
To add a new section:
1. Add a new navigation link in the `<nav>` element
2. Create a new `<section>` with a unique `id`
3. Style it using the existing CSS classes or add custom styles

### Changing Fonts
Update the `--font-primary` variable in `styles.css`:
```css
--font-primary: 'Your Font Name', sans-serif;
```

Don't forget to include the font in your HTML:
```html
<link href="https://fonts.googleapis.com/css2?family=Your+Font&display=swap" rel="stylesheet">
```

### Adding Icons
The website uses an inline SVG for the LinkedIn icon. You can add more icons:
- Use [Heroicons](https://heroicons.com/)
- Use [Font Awesome](https://fontawesome.com/)
- Use inline SVG (recommended for minimal dependencies)

## 📞 Support

If you encounter any issues:
1. Check that all files are in the same directory
2. Verify your GitHub Pages is enabled in repository settings
3. Wait a few minutes after pushing changes (GitHub Pages needs time to build)
4. Check the browser console for any JavaScript errors

## 📄 License

This template is free to use for personal and academic purposes. Feel free to customize it as needed.

---

**Good luck with your PhD applications!** 🎓
