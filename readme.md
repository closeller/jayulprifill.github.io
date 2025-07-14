# Modern Portfolio Website

A modern, responsive portfolio website with smooth animations, glassmorphism effects, and interactive elements.

## Features

- 🎨 Modern UI with glassmorphism effects
- 📱 Fully responsive design for all devices
- ✨ Smooth animations and transitions
- 🎯 Interactive project cards with parallax effect
- 📝 Contact form with validation
- 🌙 Dark mode aesthetic with neon accents
- 🔄 Dynamic background animations
- 📊 Animated skill icons
- 🚀 Performance optimized

## Getting Started

1. Clone the repository:
```bash
git clone <repository-url>
cd portfolio
```

2. Open `index.html` in your web browser to view the website.

## Customization

### Profile Information
- Edit `index.html` to update your name, bio, and project information
- Replace `assets/images/profile.jpg` with your profile picture

### Colors and Theme
The color scheme can be customized in `style.css`:
```css
:root {
    --primary-color: #2a2a72;
    --secondary-color: #009ffd;
    --accent-color: #00ff88;
    --background-dark: #0a192f;
    --text-light: #e6f1ff;
    --text-dark: #8892b0;
}
```

### Projects
Add or modify projects in the projects section of `index.html`:
```html
<div class="project-card">
    <div class="project-content">
        <h3>Project Name</h3>
        <p>Project description...</p>
        <div class="project-tech">
            <span>Technology 1</span>
            <span>Technology 2</span>
        </div>
    </div>
</div>
```

### Social Links
Update social media links in the footer section of `index.html`:
```html
<div class="social-links">
    <a href="your-github-url" target="_blank"><i class="fab fa-github"></i></a>
    <a href="your-linkedin-url" target="_blank"><i class="fab fa-linkedin"></i></a>
    <a href="your-twitter-url" target="_blank"><i class="fab fa-twitter"></i></a>
</div>
```

## Contact Form Integration

The contact form is currently set up to simulate submission. To integrate with a backend:

1. Create your backend API endpoint
2. Update the form submission code in `script.js`:
```javascript
// Replace the simulation with actual API call
try {
    const response = await fetch('your-api-endpoint', {
        method: 'POST',
        headers: {
            'Content-Type': 'application/json',
        },
        body: JSON.stringify({
            name: nameInput.value,
            email: emailInput.value,
            message: messageInput.value
        })
    });
    
    if (!response.ok) throw new Error('Failed to send message');
    
    contactForm.reset();
    showNotification('Message sent successfully!', 'success');
} catch (error) {
    showNotification('Failed to send message. Please try again.', 'error');
}
```

## Browser Support

The website is optimized for modern browsers and uses the following features:
- CSS Grid and Flexbox
- CSS Custom Properties (Variables)
- Intersection Observer API
- Modern JavaScript (ES6+)

## Performance Optimization

The website is optimized for performance:
- Minified CSS and JavaScript
- Optimized images
- Lazy loading for images
- Efficient animations using CSS transforms
- Minimal dependencies (only Font Awesome for icons)

## License

This project is open source and available under the MIT License.

## Credits

- Icons: [Font Awesome](https://fontawesome.com/)
- Fonts: [Google Fonts](https://fonts.google.com/) 