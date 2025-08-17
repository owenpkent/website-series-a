# ATDev - Series A Website

ATDev's official website showcasing our telehealth-enabled mobility devices and assistive technology solutions.

## 🏥 About ATDev

ATDev creates innovative, assistive technology that empowers people to live independently, confidently, and without barriers. Our flagship product, the Reflex smart knee brace, provides telehealth-enabled post-surgical recovery solutions.

## 🚀 Features

- **Responsive Design**: Optimized for all devices and screen sizes
- **Dark/Light Mode**: User-preferred theme with system detection
- **Modern UI**: Clean, clinical design inspired by healthcare technology
- **Interactive Animations**: VantaJS NET background effects
- **Accessibility**: WCAG compliant design patterns
- **Performance Optimized**: Fast loading with CDN resources

## 🛠 Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Styling**: Tailwind CSS
- **Fonts**: Google Fonts (Montserrat, Raleway)
- **Animations**: VantaJS, Three.js
- **Deployment**: Netlify

## 🎨 Brand Guidelines

### Colors
- **Bright Blue**: `#22A9FD` (Primary brand color)
- **Deep Blue**: `#115C90` (Secondary brand color)
- **Light Blue-Gray**: `#93C0DB` (Accent)
- **Near Black**: `#03090D` (Dark text)
- **Dark Gray**: `#606161` (Secondary text)

### Typography
- **Primary**: Montserrat (Headings, Buttons)
- **Secondary**: Raleway (Body text, Subheadings)

## 📁 Project Structure

```
website-series-a/
├── index.html          # Main website file
├── images/             # Image assets
│   └── partners/       # Partner logos (1.png - 9.png)
├── README.md           # This file
└── LICENSE            # Proprietary license
```

## 🚀 Development

### Local Development
1. Clone the repository
2. Open `index.html` in a web browser
3. For live reload, use a local server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   ```

### Deployment
The website is automatically deployed to Netlify on push to the main branch.

## 📊 Key Sections

- **Hero**: Flagship product messaging with animated background
- **Products**: Reflex Smart Knee Brace and Telehealth Platform
- **Team**: Leadership profiles with LinkedIn integration
- **Partners**: Investor and partner logos
- **Contact**: Multi-channel contact form and information

## 🔧 Configuration

### VantaJS Animation
The hero section uses VantaJS NET effect with fallback support for deployment environments:
- Automatic retry mechanism for CDN loading
- Graceful fallback to gradient background
- Error handling for production stability

### Dark Mode
Theme preference is stored in localStorage with system preference detection:
```javascript
// Theme detection
if (localStorage.getItem('theme') === 'dark' || 
    (!localStorage.getItem('theme') && 
     window.matchMedia('(prefers-color-scheme: dark)').matches)) {
    html.classList.add('dark');
}
```

## 📈 Performance

- **Optimized Images**: Compressed partner logos and assets
- **CDN Resources**: External libraries loaded from CDN
- **Lazy Loading**: Intersection Observer for animations
- **Minimal JavaScript**: Vanilla JS for optimal performance

## 🔒 Security

- **CORS Headers**: Proper cross-origin resource sharing
- **Content Security**: No inline scripts in production
- **Form Validation**: Client-side input sanitization

## 📱 Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 📞 Support

For technical issues or questions:
- **Email**: info@atdev.com
- **Website**: [atdev.com](https://atdev.com)

## 📄 License

This project is proprietary software owned by ATDev. See [LICENSE](LICENSE) for details.

---

**ATDev** - Building the Future of Mobility, Together
