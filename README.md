# Prody Admin Panel - Professional Structure

## Folder Structure (AdminLTE Style)

```
admin_panel/
├── assets/
│   ├── css/
│   │   └── style.css          # Main stylesheet
│   └── js/
│       ├── main.js             # Core JavaScript
│       └── charts.js           # Chart.js utilities
│
├── pages/
│   ├── forms/
│   │   ├── basic-forms.html    # Form elements & dropdowns
│   │   └── advanced-forms.html # Advanced form components
│   ├── tables/
│   │   ├── simple-tables.html  # Basic tables
│   │   └── data-tables.html    # Data tables with features
│   ├── ui/
│   │   ├── cards.html          # Card variations
│   │   ├── buttons.html        # Button styles
│   │   └── modals.html         # Modal components
│   ├── charts/
│   │   └── chartjs.html        # Chart.js examples
│   ├── analytics.html          # Analytics dashboard
│   ├── reports.html            # Reports page
│   ├── companies.html          # Company directory
│   └── people.html             # Team members
│
├── docs/
│   ├── README.md               # Documentation
│   └── INTEGRATION_GUIDE.md    # Framework integration
│
├── index.html                  # Project detail page
├── dashboard.html              # Main dashboard
├── welcome.html                # Welcome/landing page
├── 404.html                    # Error page
└── maintenance.html            # Maintenance page
```

## Quick Start

1. Open `welcome.html` for an overview of all pages
2. Navigate to `dashboard.html` for the main admin interface
3. Explore different sections through the sidebar navigation

## Features

### Forms (`pages/forms/`)
- ✅ Text, email, password, number inputs
- ✅ Working dropdown selects (single & multiple)
- ✅ Checkboxes and radio buttons
- ✅ Toggle switches
- ✅ File upload
- ✅ Color picker
- ✅ Range sliders
- ✅ Form validation

### UI Elements (`pages/ui/`)
- ✅ Card variations (basic, stats, profile, pricing)
- ✅ Button styles
- ✅ Modal dialogs
- ✅ Responsive layouts

### Tables (`pages/tables/`)
- ✅ Sortable tables
- ✅ Filterable data
- ✅ Pagination
- ✅ Row selection

### Charts (`pages/charts/`)
- ✅ Line charts
- ✅ Bar charts
- ✅ Doughnut charts
- ✅ Responsive charts

## Navigation Structure

The sidebar includes organized menu items with submenus:

- **Dashboard** - Main overview
- **Projects** - Project management
  - All Projects
  - New Project
- **Forms** - Form elements
  - Basic Forms
  - Advanced Forms
  - Form Validation
- **Tables** - Data tables
  - Simple Tables
  - Data Tables
- **UI Elements** - Components
  - Cards
  - Buttons
  - Modals
- **Charts** - Data visualization
  - Chart.js
  - Analytics
- **Reports** - Business reports
  - Financial
  - Sales
- **Companies** - Company directory
- **People** - Team members

## File Path Updates

All files now use relative paths based on their location:

### Root Level Files (dashboard.html, index.html, etc.)
```html
<link rel="stylesheet" href="assets/css/style.css">
<script src="assets/js/main.js"></script>
```

### Pages in `/pages/` (analytics.html, reports.html, etc.)
```html
<link rel="stylesheet" href="../assets/css/style.css">
<script src="../assets/js/main.js"></script>
```

### Pages in Subfolders (`/pages/forms/`, `/pages/ui/`, etc.)
```html
<link rel="stylesheet" href="../../assets/css/style.css">
<script src="../../assets/js/main.js"></script>
```

## Professional Features

### Working Dropdowns
All select elements are styled and functional with:
- Single selection
- Multiple selection
- Disabled states
- Size variants

### Search Functionality
- Real-time menu filtering
- Keyword-based page search
- Auto-complete suggestions

### Responsive Design
- Mobile-first approach
- Breakpoints: 768px, 1200px
- Touch-friendly interface

### Animations
- Smooth transitions
- Hover effects
- Loading states
- Number counters

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

MIT License - Free to use in personal and commercial projects

## Credits

Built with:
- HTML5 & CSS3
- Vanilla JavaScript (ES6+)
- Chart.js v4.4.1
- Material Icons
- Inter Font Family
