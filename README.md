# ⏱️ SnapStudy - Video Duration Calculator

A modern, responsive web application for calculating adjusted video playback durations with smart speed recommendations for different content types.

![SnapStudy Preview](https://img.shields.io/badge/Version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3.3-purple.svg)
![jQuery](https://img.shields.io/badge/jQuery-3.7.1-yellow.svg)

## ✨ Features

### 🎯 Core Functionality
- **Precise Time Calculations**: Convert video durations at different playback speeds
- **Real-time Updates**: Instant calculations as you type
- **Time Savings Display**: Shows exactly how much time you save or extend
- **Smart Input Handling**: Automatic overflow handling (60+ seconds → minutes, etc.)

### 🎨 Modern UI/UX
- **Glass-morphism Design**: Beautiful modern interface with backdrop blur effects
- **Dark/Light Theme Toggle**: Persistent theme switching with localStorage
- **Animated Backgrounds**: Time-themed particle effects and flowing gradients
- **Responsive Layout**: Desktop two-column, mobile accordion design
- **Smooth Animations**: Engaging micro-interactions throughout

### 📱 Responsive Design
- **Mobile-First**: Optimized for all screen sizes
- **Bootstrap 5.3.3**: Professional responsive grid system
- **Touch-Friendly**: Large, accessible input fields
- **Accordion Layout**: Collapsible details section on mobile

### 🧠 Smart Recommendations
- **12 Content Categories**: Educational, Tutorials, Documentary, Comedy, etc.
- **Speed Optimization**: Research-backed speed recommendations per category
- **Motivational Messages**: Dynamic feedback based on time saved
- **Visual Feedback**: Color-coded speed badges showing optimal ranges

## 🚀 Quick Start

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Local web server (optional, for AJAX features)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/kanishkaGayan/snapstudy.git
   cd snapstudy
   ```

2. **Open in browser**
   ```bash
   # Option 1: Direct file access
   open index.html
   
   # Option 2: Local server (recommended)
   python -m http.server 8000
   # Then visit: http://localhost:8000
   ```

3. **Start calculating!**
   - Enter your video duration (hours, minutes, seconds)
   - Select playback speed
   - Get instant time calculations and recommendations

## 🎮 Usage

### Basic Calculation
1. **Input Duration**: Enter your video's original length
2. **Select Speed**: Choose from 0.25× to 3× playback speeds
3. **View Results**: See adjusted duration and time saved/extended

### Smart Recommendations
1. **Choose Category**: Select your video type from the dropdown
2. **Get Insights**: View optimal speed ranges for your content
3. **Apply Tips**: Follow research-backed recommendations

### Theme Switching
- Click the theme toggle button (☀️/🌙) in the top-right corner
- Your preference is automatically saved

## 🏗️ Technical Stack

### Frontend Technologies
- **HTML5**: Semantic markup structure
- **CSS3**: Custom properties, animations, responsive design
- **JavaScript (ES6+)**: Modern syntax with jQuery
- **Bootstrap 5.3.3**: CSS framework and components
- **jQuery 3.7.1**: DOM manipulation and AJAX

### Design System
- **CSS Custom Properties**: Unified theming system
- **Google Fonts**: Inter (UI) + JetBrains Mono (code/numbers)
- **Color Palette**: Purple/blue gradient with accent colors
- **Animation Library**: Custom keyframe animations

### Features Implementation
- **AJAX**: Dynamic loading of playback speeds from JSON
- **localStorage**: Theme persistence across sessions
- **Responsive Grid**: Bootstrap's 12-column system
- **Component Architecture**: Modular CSS and JS structure

## 📁 Project Structure

```
snapstudy-calculator/
├── index.html          # Main application file
├── speeds.json         # Playback speed options data
├── README.md          # This file
└── assets/            # (Future: images, icons)
```

## 🎨 Customization

### Color Themes
Edit CSS custom properties in `:root` and `[data-theme="dark"]`:
```css
:root {
  --primary: #6366f1;     /* Main accent color */
  --secondary: #8b5cf6;   /* Secondary accent */
  --accent: #06b6d4;      /* Highlight color */
}
```

### Speed Options
Modify `speeds.json` to add/remove playback speeds:
```json
[
  {"value": "1.5", "label": "1.5× Fast"},
  {"value": "2", "label": "2× Double Speed"}
]
```

### Categories
Add new video categories in the `categoryRecommendations` object:
```javascript
newCategory: {
  title: "Your Category",
  tip: "Speed recommendation tip",
  optimalSpeeds: ["1×", "1.25×", "1.5×"]
}
```

## 🌟 Use Cases

### Students & Learners
- **Lecture Videos**: Start at 1× for new topics, 1.25-1.5× for review
- **Tutorial Following**: Use 1× when coding along, faster for review
- **Language Learning**: 0.75× for pronunciation, normal for fluency

### Content Consumers
- **Podcast Efficiency**: Most people comfortable at 1.5-2× speed
- **News Consumption**: 1.5-2× for information gathering
- **Entertainment**: Maintain 1× for comedy timing, 1.25× max for movies

### Professionals
- **Meeting Recordings**: 1.5-1.75× for review sessions
- **Training Materials**: Variable speeds based on complexity
- **Research Content**: Faster speeds for familiar topics

## 🤝 Contributing

Contributions are welcome! Here's how to get started:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Make your changes**
4. **Test thoroughly**
5. **Commit changes**: `git commit -m 'Add amazing feature'`
6. **Push to branch**: `git push origin feature/amazing-feature`
7. **Open a Pull Request**

### Development Guidelines
- Follow existing code style and structure
- Test on multiple browsers and screen sizes
- Update README if adding new features
- Keep animations smooth and purposeful

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Bootstrap Team**: For the excellent CSS framework
- **jQuery Foundation**: For the powerful JavaScript library
- **Google Fonts**: For beautiful typography options
- **Research Sources**: Academic studies on video playback speed comprehension

## 📊 Browser Support

- ✅ Chrome 80+
- ✅ Firefox 75+
- ✅ Safari 13+
- ✅ Edge 80+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🔮 Future Enhancements

- [ ] Video file upload for automatic duration detection
- [ ] Playlist duration calculations
- [ ] Export results to CSV/PDF
- [ ] Browser extension version
- [ ] API integration with video platforms
- [ ] Advanced analytics and usage tracking
- [ ] Collaborative playlists with shared calculations

---

**Made with ❤️ for efficient learning and content consumption**

*Time is your most valuable resource - use it wisely!*
