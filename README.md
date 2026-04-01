# QSTP Innovation Hub

A modern dashboard application for Qatar Science & Technology Park (QSTP) company data.

## Features

- 🔐 **Simple Password Protection** - Basic authentication with password: `qstp2024`
- 📊 **Interactive Dashboard** - KPI cards and charts showing key metrics
- 🏢 **Company Directory** - Searchable and filterable table of all companies
- 👥 **Company Details** - Drill-down pages with full company info and founders
- 📱 **Responsive Design** - Works on desktop, tablet, and mobile

## Dashboard Metrics

- Total Companies (Enterprises & Startups)
- Active Companies
- Total Employees
- Qatari Employees
- Total Revenue (2024)
- Total Investment (2024)

## Charts Included

1. Companies by Industry
2. Enterprises vs Startups (pie chart)
3. Companies by Status
4. Funding Stage Distribution
5. Employee Gender Distribution
6. Top 10 Companies by Revenue

## Files Structure

```
QSTP_Site/
├── index.html           # Main application (single-page app)
├── QSTP_Companies.csv   # Company data
├── Founders.csv         # Founders data
└── README.md           # This file
```

## Deployment to Netlify

### Option 1: Drag & Drop

1. Go to [Netlify Drop](https://app.netlify.com/drop)
2. Drag the entire `QSTP_Site` folder onto the page
3. Your site will be live in seconds!

### Option 2: GitHub Integration

1. Push this folder to a GitHub repository
2. Go to [Netlify](https://app.netlify.com)
3. Click "Add new site" → "Import an existing project"
4. Connect to GitHub and select your repository
5. Click "Deploy"

### Option 3: Netlify CLI

```bash
# Install Netlify CLI
npm install -g netlify-cli

# Login to Netlify
netlify login

# Deploy
cd QSTP_Site
netlify deploy --prod
```

## Customization

### Change Password

Edit `index.html` and find this line:
```javascript
const APP_PASSWORD = 'qstp2024';
```
Change `qstp2024` to your desired password.

### Update Data

Replace the CSV files with updated data. The column structure must remain the same.

### Customize Colors

Edit the CSS variables at the top of `index.html`:
```css
:root {
    --primary: #0a2647;
    --secondary: #144272;
    --accent: #2c7da0;
    /* ... */
}
```

## Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge

## Technologies Used

- HTML5 / CSS3
- Vanilla JavaScript
- [Chart.js](https://www.chartjs.org/) - For charts

## License

Internal use only - QSTP
