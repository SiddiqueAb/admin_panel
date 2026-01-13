# Prody Admin Panel

A complete, modern, and responsive static admin panel built with HTML, CSS, and vanilla JavaScript. Perfect for managing projects, analytics, companies, and teams.

## 📁 File Structure

```
admin_panel/
├── index.html              # Project detail page (House Spectrum Ltd)
├── dashboard.html          # Main dashboard
├── analytics.html          # Analytics page
├── reports.html            # Reports page (coming soon)
├── companies.html          # Companies directory
├── people.html             # Team members page
├── 404.html               # 404 error page
├── maintenance.html       # Maintenance mode page
├── style.css              # Main stylesheet (reusable across project)
├── js/
│   ├── main.js           # Main JavaScript functionality
│   └── charts.js         # Chart configurations
└── README.md             # This file
```

## ✨ Features

### 🎨 **Design & UI**
- **Pixel-perfect design** matching the reference
- **Fully responsive** - Works on desktop, tablet, and mobile
- **Smooth animations** - Fade-ins, slides, and transitions
- **Modern card-based layout**
- **Professional color scheme** with CSS variables

### 🔍 **Search Functionality**
- **Smart search** with suggestions
- **Keyboard navigation** (Arrow keys, Enter)
- **Categorized results**
- **Highlighted matches**

### 🗂️ **Navigation**
- **Collapsible submenus**
- **Active page highlighting**
- **Mobile-friendly sidebar**
- **Breadcrumb navigation**

### 📊 **Charts**
- **Interactive charts** using Chart.js
- **Budget tracking** (line chart)
- **Sales overview** (line chart)
- **Traffic sources** (doughnut chart)
- **Weekly visitors** (bar chart)
- **Analytics tracking** (multi-line chart)

### 📋 **Tables**
- **Sortable columns**
- **Row selection** with checkboxes
- **Pagination**
- **Search/filter**
- **Export functionality**

### 🎯 **Dropdowns & Modals**
- **Fully functional dropdowns**
- **Modal dialogs**
- **Click-outside to close**
- **ESC key support**

### 🔔 **Notifications**
- **Toast notifications**
- **Auto-dismiss**
- **Multiple types** (success, error, warning, info)

### 🎭 **Animations**
- **Scroll animations** (fade-in-up)
- **Number counters**
- **Hover effects**
- **Smooth transitions**

## 🚀 Getting Started

### Quick Start
1. **No installation required!** Just open any HTML file in your browser
2. **Start with** `dashboard.html` for the main dashboard
3. **Or open** `index.html` for the project detail page

### For Development
1. Open the folder in VS Code or your favorite editor
2. Use Live Server extension for auto-reload
3. Modify `style.css` for styling changes
4. Edit JavaScript files in `/js` folder

## 📖 Usage Guide

### Navigation
- **Sidebar menu** - Click items to navigate
- **Submenus** - Click parent items with arrow to expand
- **Mobile** - Click hamburger icon to toggle sidebar
- **Search** - Type in search box for suggestions

### Customization

#### Colors
Edit CSS variables in `style.css`:
```css
:root {
    --primary-color: #3b82f6;
    --accent-red: #ef4444;
    --accent-green: #10b981;
    /* ... more colors */
}
```

#### Fonts
Change font family:
```css
body {
    font-family: 'Inter', sans-serif;
}
```

#### Layout
Adjust sidebar width:
```css
:root {
    --sidebar-width: 240px;
}
```

### Adding New Pages
1. Copy any existing page as template
2. Update the `<title>` tag
3. Update active class in sidebar navigation
4. Customize the content area
5. Include scripts at the bottom

### Charts
Charts use Chart.js. Modify configurations in `js/charts.js`:
```javascript
createBudgetChart(canvas) {
    return new Chart(ctx, {
        type: 'line',
        data: { /* your data */ },
        options: { /* your options */ }
    });
}
```

## 📄 Page Descriptions

### Dashboard (`dashboard.html`)
- **Stats cards** - Revenue, Orders, Customers, Projects
- **Sales chart** - Year-over-year sales
- **Traffic sources** - Pie chart breakdown
- **Recent activity** - Latest actions
- **Top products** - Best sellers

### Projects (`index.html`)
- **Project header** - Name, status, stats
- **Budget chart** - Revenue vs Expenditures
- **Deals table** - All project deals
- **Interactive controls** - Filter, sort, export

### Analytics (`analytics.html`)
- **Key metrics** - Page views, visitors, bounce rate
- **Traffic analysis** - 30-day trend chart
- **Device breakdown** - Desktop vs mobile
- **Top pages** - Most visited pages

### Companies (`companies.html`)
- **Company directory** - All business partners
- **Detailed info** - Industry, location, employees
- **Status tracking** - Active, pending, inactive
- **Search & filter** - Find companies quickly

### People (`people.html`)
- **Team grid** - Card-based layout
- **Contact info** - Email and phone
- **Online status** - Real-time indicators
- **Quick actions** - Email, call, more options

### 404 Page (`404.html`)
- **Error display** - Large 404 code
- **Helpful message** - User-friendly text
- **Navigation buttons** - Go back or home

### Maintenance (`maintenance.html`)
- **Countdown timer** - Time remaining
- **Professional message** - Inform users
- **Branded design** - Consistent styling

## 🎨 CSS Architecture

### Organization
The CSS is organized into logical sections:
1. **Global Styles** - Reset, variables, base styles
2. **Sidebar** - Navigation and menu
3. **Main Content** - Page layouts
4. **Components** - Reusable elements
5. **Utilities** - Helper classes
6. **Responsive** - Media queries

### CSS Variables
All colors, spacing, and design tokens are defined as CSS variables for easy customization.

### Utility Classes
Use utility classes for quick styling:
```html
<div class="flex items-center gap-3 p-4 rounded-lg shadow-md">
    <!-- Content -->
</div>
```

## 🔧 JavaScript Features

### Main.js
- **AdminPanel class** - Core functionality
- **Sidebar management** - Toggle, active states
- **Search system** - Suggestions, keyboard nav
- **Dropdowns** - Dynamic positioning
- **Modals** - Show/hide logic
- **Animations** - Scroll observers
- **Notifications** - Toast system

### Charts.js
- **ChartManager class** - All charts
- **Multiple chart types** - Line, bar, doughnut
- **Responsive** - Auto-resize
- **Customizable** - Easy to modify

### TableManager
- **Sorting** - Click headers to sort
- **Filtering** - Search within tables
- **Selection** - Select all/individual
- **Pagination** - Navigate pages

## 🌐 Browser Support
- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)

## 📱 Responsive Breakpoints
- **Desktop**: 1200px+
- **Tablet**: 768px - 1199px
- **Mobile**: < 768px

## 🎯 Best Practices
- **Semantic HTML** - Proper element usage
- **Accessible** - ARIA labels where needed
- **Performance** - Optimized animations
- **Clean code** - Well-commented and organized
- **Reusable** - Component-based approach

## 🔄 Updates & Maintenance
To add new features:
1. **Pages** - Create new HTML using existing templates
2. **Styles** - Add to appropriate section in style.css
3. **Scripts** - Add functions to main.js or create new files
4. **Charts** - Add chart methods to charts.js

## 💡 Tips
- **Customize colors** - Edit CSS variables for instant theme changes
- **Add pages** - Copy existing pages and modify
- **Extend functionality** - Add to AdminPanel class
- **Create components** - Use utility classes for consistency

## 🤝 Contributing
Feel free to customize this admin panel for your projects! Suggestions for improvements are welcome.

## 📝 License
Free to use for personal and commercial projects.

## 🎉 Credits
Built with:
- **HTML5** - Structure
- **CSS3** - Styling
- **JavaScript (ES6+)** - Functionality
- **Chart.js** - Data visualization
- **Google Fonts** - Inter font family
- **Material Icons** - Icon set

---

**Prody Admin Panel** - Professional, Modern, Responsive ✨
