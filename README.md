# CSV Plumbing Website

A professional, responsive website for CSV Plumbing, Drainage & Gasfitting - serving Blue Mountains and Greater Western Sydney.

## About

This is a GitHub Pages hosted website for CSV Plumbing. It features:

- **Hero Section** - Eye-catching header with call-to-action
- **Why Choose Us** - Key benefits and value propositions
- **Services Grid** - All plumbing services offered
- **Contact Form** - Easy way for customers to request quotes
- **Responsive Design** - Works perfectly on desktop, tablet, and mobile

## Services Offered

- General Plumbing
- Blocked Drains
- Leak Detection
- Hot Water Systems
- Bathroom Repairs
- Gas Fitting
- Gas Leaks
- Shower Sealing

## Contact

- **Phone:** 0450 207 705
- **Email:** chris@csvplumbing.com
- **Service Area:** Blue Mountains & Greater Western Sydney

## Setup Instructions

### Local Development

1. Clone or download this repository
2. Open `index.html` in your web browser
3. For local development, you can use Python's built-in server:
   ```bash
   python3 -m http.server 8000
   ```
   Then visit `http://localhost:8000` in your browser

### Deploying to GitHub Pages

1. Create a repository on GitHub named `csvplumbing.github.io` (or use your actual GitHub username)
2. Push these files to the repository
3. Your site will be live at `https://csvplumbing.github.io`

**To use a custom domain:**
1. Add a `CNAME` file with your domain name (e.g., `csvplumbing.com.au`)
2. Configure your domain registrar to point to GitHub Pages

## Customization

### Colors

The site uses CSS variables that can be easily customized in `style.css`:

```css
:root {
    --primary-blue: #4485b1;
    --secondary-blue: #407db1;
    --white: #ffffff;
    --black: #000000;
    --accent: #ff9800;
}
```

### Contact Form

The contact form uses Formspree.io for submissions. To enable it:

1. Go to [formspree.io](https://formspree.io)
2. Create a new form and get your Form ID
3. In `index.html`, replace `YOUR_FORM_ID` in the form action with your actual ID

Example:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

## File Structure

```
├── index.html           # Main website page
├── style.css            # All styling
├── README.md            # This file
└── CNAME                # Custom domain (optional)
```

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## License

© 2024 CSV Plumbing, Drainage & Gasfitting. All rights reserved.

## Contact for Updates

For any changes or updates to the website, contact the site administrator.
