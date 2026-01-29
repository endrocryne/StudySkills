# UI Framework - Reusable Web App Starter

A lightweight, beautiful, and accessible UI framework extracted from the DMHS AI Time Tracker. Build modern web applications with three stunning design systems: Material 3, Fluent Design, and Liquid Glass.

![License](https://img.shields.io/badge/license-Mishra--CSIL--2025-blue)
![Version](https://img.shields.io/badge/version-1.0.0-green)

## ✨ Features

- **Three Design Systems**: Switch between Google Material 3, Microsoft Fluent Design, and Liquid Glass aesthetics
- **Complete Theming**: Light, Dark, and High Contrast themes with custom accent colors
- **Drag & Drop Customization**: Rearrange and resize UI elements in real-time
- **Layout Persistence**: Save custom layouts to localStorage
- **Zero Dependencies**: Pure HTML, CSS, and JavaScript (only Material Icons for icons)
- **Mobile-First**: Responsive design that works on all devices
- **Accessible**: Built with WCAG guidelines in mind
- **Easy to Use**: Simple API and clear documentation
- **Highly Customizable**: CSS variables for easy theming

## 🚀 Quick Start

### Include Framework Files

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My App</title>
    <link rel="stylesheet" href="framework.css">
    <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
</head>
<body class="liquid-glass" data-theme="light">
    <!-- Your content -->
    <script src="framework.js"></script>
    <script src="customizer.js"></script>
</body>
</html>
```

### 2. Initialize the Framework

```javascript
const app = new UIFramework({
    appName: 'My Application',
    defaultTheme: 'light',
    defaultStyle: 'liquid-glass'
});
```

### 3. Build Your App

Use the starter template or examples to get started quickly!

## 📁 File Structure

```
ui-framework/
├── framework.css           # Core CSS styles
├── framework.js            # Core JavaScript functionality
├── customizer.js           # Drag-and-drop customization module
├── starter-template.html   # Clean starter template
├── FRAMEWORK-GUIDE.md      # Comprehensive documentation
├── README.md              # This file
└── examples/
    ├── simple-timer/      # Example: Timer/Stopwatch app
    │   └── index.html
    └── dashboard/         # Example: Complex dashboard
        └── index.html
```

## 🎨 Design Systems

### Material 3
Google's modern design language with smooth animations, rounded corners, and elevation.

```html
<body class="material3" data-theme="light">
```

**Best for**: Modern consumer apps, creative tools, media applications

### Fluent Design
Microsoft's clean, efficient design with sharp corners and instant feedback.

```html
<body class="fluent" data-theme="light">
```

**Best for**: Professional tools, enterprise applications, productivity apps

### Liquid Glass
Modern glassmorphism with backdrop blur, floating elements, and fluid animations.

```html
<body class="liquid-glass" data-theme="light">
```

**Best for**: Premium apps, portfolios, modern web experiences

## 🌈 Themes

Switch between three built-in themes:

- **Light Theme**: Clean and professional (default)
- **Dark Theme**: Easy on the eyes in low-light
- **High Contrast**: Maximum accessibility

```javascript
// Programmatically change theme
document.body.setAttribute('data-theme', 'dark');
```

## 🎯 Core Components

### Header & Navigation
```html
<div class="header">
    <div class="title">App Name</div>
    <div class="controls">
        <button id="settingsBtn">⚙️ Settings</button>
    </div>
</div>
```

### Tab System
```html
<div class="tabs">
    <button class="tab-link active" onclick="openTab(event, 'home')">
        <i class="material-icons">home</i> Home
    </button>
</div>

<div id="home" class="tab-content" style="display: block;">
    <!-- Content -->
</div>
```

### Layout Customization (NEW!)
Enable drag-and-drop customization in settings:
```javascript
// Customization is automatically enabled when you include customizer.js
// Users can toggle it in Settings > Customize Layout
```

Features:
- **Drag to Reorder**: Click and drag elements to rearrange them
- **Resize Elements**: Use the resize handle (⋰) in bottom-right corner
- **Persistent Layouts**: Saved automatically to localStorage
- **Reset Option**: Restore default layout anytime

### Modal Dialogs
```html
<div class="modal" id="myModal">
    <div class="modal-content">
        <div class="modal-header">
            <div class="modal-title">Title</div>
            <button class="close-btn">&times;</button>
        </div>
        <!-- Modal content -->
    </div>
</div>
```

### Forms
```html
<div class="form-group">
    <label for="input">Label:</label>
    <input type="text" id="input">
</div>
```

## 📚 Examples

### Simple Timer Application
A complete timer/stopwatch app demonstrating:
- Multiple tabs
- Local storage
- Custom styling
- User interactions

[View Example](examples/simple-timer/index.html)

### Dashboard Application
A complex dashboard showcasing:
- Data visualization placeholders
- Responsive grid layouts
- Tables and cards
- Notification system

[View Example](examples/dashboard/index.html)

## 🛠️ Customization

### Change Accent Color
```javascript
app.setAccentColor('#e91e63');
```

### Custom CSS Variables
```css
:root {
    --primary: #1976d2;
    --background: #ffffff;
    --border-radius: 8px;
}
```

### Override Styles
```css
/* Your custom styles */
.my-custom-button {
    background: linear-gradient(45deg, #667eea 0%, #764ba2 100%);
}
```

## 📖 Documentation

For detailed documentation, best practices, and advanced usage, see [FRAMEWORK-GUIDE.md](FRAMEWORK-GUIDE.md).

Topics covered:
- Getting started
- Design system details
- Component reference
- Theming and customization
- Layout patterns
- Best practices
- Accessibility guidelines
- Performance optimization
- Troubleshooting

## 🎓 Learning Path

1. **Start with the basics**: Open `starter-template.html` in your browser
2. **Explore examples**: Check out the timer and dashboard examples
3. **Read the guide**: Review `FRAMEWORK-GUIDE.md` for best practices
4. **Build something**: Create your own app using the framework
5. **Customize**: Adjust colors, fonts, and styles to match your brand

## 🏗️ Building Your App

### Step 1: Choose Your Template
- Use `starter-template.html` for a clean slate
- Copy an example as a starting point

### Step 2: Customize
- Update the app name
- Modify tab structure
- Add your content

### Step 3: Style
- Choose a design system
- Pick a theme
- Set accent colors

### Step 4: Add Functionality
- Write your app logic
- Handle user interactions
- Store data with localStorage

## 💡 Use Cases

This framework is perfect for:

- ✅ **Timers & Clocks**: Countdown timers, stopwatches, world clocks
- ✅ **Dashboards**: Analytics, monitoring, admin panels
- ✅ **Tools**: Calculators, converters, generators
- ✅ **Productivity**: Todo lists, note-taking, habit trackers
- ✅ **Content**: Blogs, portfolios, documentation sites
- ✅ **Education**: Learning apps, quizzes, tutorials
- ✅ **Business**: CRM tools, inventory systems, booking systems
- ✅ **Entertainment**: Games, media players, social apps

## 🌐 Browser Support

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers

**Note**: Liquid Glass mode requires backdrop-filter support (most modern browsers).

## ♿ Accessibility

The framework follows WCAG 2.1 guidelines:

- ✅ Keyboard navigation support
- ✅ Screen reader compatible
- ✅ High contrast mode
- ✅ Color contrast ratios meet AA standards
- ✅ Semantic HTML
- ✅ ARIA labels where appropriate

## 📱 Responsive Design

The framework is mobile-first and fully responsive:

- **Mobile**: Optimized touch targets, simplified layouts
- **Tablet**: Adaptive grid systems, enhanced navigation
- **Desktop**: Full feature set, multi-column layouts

## 🔧 Requirements

- Modern web browser
- Basic HTML, CSS, JavaScript knowledge
- Text editor or IDE
- (Optional) Local web server for development

## 📦 What's Included

- `framework.css` (11KB) - All styles for three design systems
- `framework.js` (11KB) - Core functionality and utilities
- `starter-template.html` (4KB) - Ready-to-use template
- `FRAMEWORK-GUIDE.md` (17KB) - Complete documentation
- 2 complete example applications

**Total Size**: ~58KB (uncompressed, excluding examples)

## 🚦 Getting Help

1. **Read the guide**: Most questions are answered in `FRAMEWORK-GUIDE.md`
2. **Check examples**: See how features are implemented
3. **Inspect the code**: The framework is well-commented
4. **Experiment**: Try things in the browser console

## 🤝 Contributing

This framework was extracted from the DMHS AI Time Tracker project. To contribute:

1. Test your changes in all three design systems
2. Ensure accessibility is maintained
3. Document new features
4. Follow existing code style

## 📝 License

This framework is part of the DMHS AI Time Tracker project and is covered under the Mishra-CSIL-2025 License.

## 👥 Credits

**Original Application**: DMHS AI Time Tracker  
**Developers**: Agastya Mishra, Pratham Tippi, Dhiraj Javvadi, Siddhant Shukla  
**Framework Extraction**: Based on shared code from DMHS AI (https://dmhs-ai.gt.tc)

## 🎉 Showcase

Built something cool with this framework? We'd love to see it!

## 📊 Version History

### v1.0.0 (January 2026)
- Initial release
- Three design systems (Material 3, Fluent, Liquid Glass)
- Complete theming system
- Responsive layouts
- Accessibility features
- Example applications
- Comprehensive documentation

---

**Ready to build something amazing? Start with `starter-template.html` and let your creativity flow! 🚀**

For questions or feedback, refer to the main DMHS AI Time Tracker repository.
