# TaskFlow Landing Page - Deployment Guide

## Quick Start Deployment to Netlify

### Option 1: Deploy via Netlify Web UI (Recommended)

1. **Create a GitHub Repository**
   ```bash
   cd /home/ubuntu/TaskFlowApp-Landing
   git remote add origin https://github.com/osasbenny/TaskFlowApp-Landing.git
   git branch -M main
   git push -u origin main
   ```

2. **Connect to Netlify**
   - Go to [netlify.com](https://netlify.com)
   - Click "New site from Git"
   - Select GitHub and authorize
   - Choose `TaskFlowApp-Landing` repository
   - Build settings:
     - Build command: (leave empty)
     - Publish directory: `.` (root)
   - Click "Deploy site"

3. **Configure Custom Domain**
   - In Netlify dashboard, go to "Domain settings"
   - Add your custom domain (e.g., `taskflowapp.com`)
   - Follow DNS configuration instructions

### Option 2: Deploy via Netlify CLI

```bash
# Install Netlify CLI
npm install -g netlify-cli

# Login to Netlify
netlify login

# Deploy
cd /home/ubuntu/TaskFlowApp-Landing
netlify deploy --prod
```

### Option 3: Deploy via Vercel (Alternative)

```bash
# Install Vercel CLI
npm install -g vercel

# Deploy
cd /home/ubuntu/TaskFlowApp-Landing
vercel --prod
```

## Post-Deployment Checklist

- [ ] Landing page loads without errors
- [ ] All navigation links work
- [ ] Screenshots display correctly
- [ ] Privacy policy page is accessible
- [ ] Footer credit link works
- [ ] Mobile responsive design works
- [ ] Google Play Store link is correct
- [ ] SSL certificate is active (HTTPS)
- [ ] Custom domain is configured (if applicable)

## Environment Variables

No environment variables are required for this static site.

## Performance Optimization

The site is already optimized with:
- Minified CSS and JavaScript
- Optimized image assets
- Caching headers configured in `netlify.toml`
- Fast static file serving

## Monitoring

After deployment, monitor:
- Page load times
- Core Web Vitals
- 404 errors
- Traffic patterns

Use Netlify Analytics or Google Analytics to track performance.

## Troubleshooting

### Images Not Loading
- Ensure image paths are relative
- Check that asset files exist in the correct directories
- Verify file permissions

### Links Not Working
- Check that all href attributes are correct
- Verify relative paths match directory structure
- Test on both desktop and mobile

### Styling Issues
- Clear browser cache (Ctrl+Shift+Delete)
- Check CSS file paths
- Verify Netlify cache is cleared

## Updating Content

To update the landing page:

1. Edit HTML files locally
2. Update screenshots in `assets/screenshots/`
3. Modify CSS in `css/` directory
4. Commit changes: `git add . && git commit -m "Update content"`
5. Push to GitHub: `git push origin main`
6. Netlify will automatically redeploy

## Support

For deployment issues:
- Check Netlify documentation: https://docs.netlify.com
- Review build logs in Netlify dashboard
- Contact Netlify support if needed

## Security

- All traffic is HTTPS encrypted
- Security headers are configured
- No sensitive data is stored
- Privacy policy is comprehensive and compliant

---

**Last Updated:** March 18, 2026
