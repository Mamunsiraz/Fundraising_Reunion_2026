# Donation Management System 💝

A modern, responsive web-based donation management system with transparent tracking of funding and expenditures.

## 🌟 Features

### Funding Dashboard
- **Interactive Leaderboard** with top donor rankings
- **Medal System** (🥇🥈🥉) for top 3 donors
- **Animated Progress Bars** showing donation amounts
- **Real-time Statistics** with donor counts and totals
- **Responsive Design** for all devices

### Expenditure Dashboard
- **Expense Distribution Charts** with donut visualization
- **Category Breakdown** with progress tracking
- **Recent Transactions Table** with status badges
- **Budget Monitoring** and remaining funds tracking
- **Multi-period Views** (Month/Quarter/Year)

## 📁 Project Structure

```
donation-system/
├── index.html          # Homepage with navigation
├── funding.html        # Funding/Donation Dashboard
├── expenditure.html    # Expenditure Dashboard
└── README.md          # This file
```

## 🚀 Quick Start

### Local Development

1. Clone this repository:
```bash
git clone https://github.com/yourusername/donation-system.git
cd donation-system
```

2. Open `index.html` in your web browser

### GitHub Pages Deployment

1. **Create a GitHub repository** for your project

2. **Upload files** to your repository:
   - index.html
   - funding.html
   - expenditure.html
   - README.md

3. **Enable GitHub Pages**:
   - Go to your repository settings
   - Navigate to "Pages" section
   - Under "Source", select "main" branch
   - Click "Save"

4. **Access your site**:
   - Your site will be available at: `https://yourusername.github.io/repository-name/`

## 📱 Responsive Design

The system is fully responsive and works on:
- 💻 Desktop (1400px+)
- 📱 Tablet (768px - 1200px)
- 📱 Mobile (320px - 768px)

## 🎨 Design Features

- **Modern UI** with Inter font family
- **Gradient Backgrounds** and smooth animations
- **Card-based Layouts** with hover effects
- **Color-coded Categories** for easy navigation
- **Interactive Charts** with real-time updates

## 🛠️ Customization

### Update Data

To update donation or expenditure data, edit the HTML files:

**funding.html** - Update donor information:
```html
<div class="donor-name">Your Donor Name</div>
<div class="donation-amount">$XX,XXX</div>
```

**expenditure.html** - Update expense categories:
```html
<div class="category-name">Category Name</div>
<div class="category-amount">$XX,XXX</div>
```

### Change Colors

Modify the gradient colors in the `<style>` section:
```css
background: linear-gradient(135deg, #your-color1 0%, #your-color2 100%);
```

### Update Logo

Change the logo text in the navigation:
```html
<div class="logo">Your Organization Name</div>
```

## 📊 Data Sources

Currently using placeholder data. To connect to real data:

1. **Backend Integration**: Create API endpoints for donations and expenses
2. **Database Connection**: Connect to MySQL/PostgreSQL/MongoDB
3. **JavaScript Fetch**: Update data dynamically using AJAX/Fetch API

Example:
```javascript
fetch('/api/donations')
  .then(response => response.json())
  .then(data => updateDashboard(data));
```

## 🔒 Security Notes

- This is a frontend-only implementation
- For production, implement proper backend authentication
- Sanitize all user inputs
- Use HTTPS for deployment
- Implement CORS policies if needed

## 🌐 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers

## 📝 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📧 Contact

For questions or support, please open an issue on GitHub.

## 🙏 Acknowledgments

- Icons: Emoji Unicode
- Fonts: Google Fonts (Inter)
- Design: Modern dashboard principles
- Images: Pravatar.cc (placeholder avatars)

---

Made with ❤️ for transparent charitable giving
