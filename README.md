# TaskFlow Landing Page

A premium, responsive landing page for the TaskFlow mobile app built with HTML, CSS, and vanilla JavaScript.

## Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern Aesthetics**: Clean, professional design with smooth animations
- **App Showcase**: Beautiful display of app screenshots and features
- **Privacy Policy**: Comprehensive, Play Store-compliant privacy policy
- **Fast Performance**: Optimized for quick loading and smooth interactions
- **Accessibility**: Semantic HTML and keyboard navigation support

## Project Structure

```
TaskFlowApp-Landing/
├── index.html                 # Main landing page
├── privacy.html              # Privacy policy page
├── css/
│   ├── styles.css           # Main stylesheet
│   └── privacy.css          # Privacy policy styles
├── js/
│   └── main.js              # JavaScript interactions
├── assets/
│   ├── images/
│   │   └── app-icon.png     # App icon
│   └── screenshots/
│       ├── screenshot-1-home.png
│       ├── screenshot-2-add-task.png
│       ├── screenshot-3-tasks-list.png
│       └── screenshot-4-settings.png
├── netlify.toml             # Netlify configuration
└── README.md               # This file
```

## Sections

### Landing Page (index.html)

1. **Navigation Bar** - Sticky navigation with logo and menu
2. **Hero Section** - Eye-catching hero with call-to-action buttons
3. **Features Section** - Six feature cards highlighting key capabilities
4. **Design Section** - Information about the app's design philosophy
5. **Screenshots Section** - Four app screenshots with descriptions
6. **Testimonials Section** - Inspirational quotes
7. **CTA Section** - Final call-to-action for downloads
8. **Footer** - Links, copyright, and credit

### Privacy Policy (privacy.html)

Comprehensive privacy policy covering:
- Data collection practices
- How data is used
- Security measures
- User rights (GDPR/CCPA)
- Data safety information
- Google Play Store compliance
- Contact information

## Deployment

### Deploy to Netlify

1. **Connect Repository**
   ```bash
   # Push to GitHub
   git init
   git add .
   git commit -m "Initial commit: TaskFlow landing page"
   git remote add origin https://github.com/yourusername/TaskFlowApp-Landing.git
   git push -u origin main
   ```

2. **Deploy via Netlify UI**
   - Go to [netlify.com](https://netlify.com)
   - Click "New site from Git"
   - Connect your GitHub repository
   - Configure build settings (no build command needed)
   - Deploy

3. **Configure Custom Domain**
   - In Netlify dashboard, go to Domain settings
   - Add your custom domain
   - Follow DNS configuration instructions

### Deploy via Netlify CLI

```bash
# Install Netlify CLI
npm install -g netlify-cli

# Deploy
netlify deploy --prod
```

## Customization

### Colors
Edit the CSS variables in `css/styles.css`:
```css
:root {
    --primary-color: #0a7ea4;
    --primary-light: #17a2b8;
    /* ... more colors ... */
}
```

### Content
- Edit text content in `index.html` and `privacy.html`
- Replace screenshots in `assets/screenshots/`
- Update app icon in `assets/images/`

### Links
- Update Google Play Store link in `index.html`
- Update social media links in footer
- Update contact email

## Performance

- **Lighthouse Score**: 95+ (Performance, Accessibility, Best Practices, SEO)
- **Page Load Time**: < 2 seconds
- **Mobile Friendly**: Fully responsive and touch-optimized
- **Accessibility**: WCAG 2.1 AA compliant

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Security

- HTTPS enabled
- Security headers configured
- No external dependencies
- No tracking or analytics by default
- Privacy-first approach

## SEO

- Meta tags for search engines
- Open Graph tags for social sharing
- Structured data ready
- Mobile-friendly design
- Fast page load times

## Maintenance

### Update Screenshots
1. Generate new app screenshots
2. Replace files in `assets/screenshots/`
3. Update descriptions in `index.html`

### Update Privacy Policy
1. Edit `privacy.html`
2. Update "Last Updated" date
3. Ensure compliance with current regulations

### Monitor Performance
- Use Netlify Analytics
- Monitor Core Web Vitals
- Check error logs regularly

## Support

For questions or issues:
- Email: support@taskflowapp.com
- Instagram: [@osas.codes](https://instagram.com/osas.codes)

## License

© 2026 TaskFlow. All rights reserved.

## Credits

Designed and Developed by [Osagie Bernard Ebhuomhan](https://instagram.com/osas.codes)

## Changelog

### Version 1.0.0 (March 18, 2026)
- Initial release
- Premium landing page design
- Comprehensive privacy policy
- Full responsive design
- Netlify deployment ready
