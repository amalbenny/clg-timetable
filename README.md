# Daily Timetable PWA

---
📌 *Notice* : This repository is longer maintained for shifting focus to [amalbenny/class-timetable](https://github.com/amalbenny/class-timetable/).
---
A lightweight Progressive Web App (PWA) for displaying your daily timetable with subject types and timing information.

## Features

- 📱 **Progressive Web App** - Works offline and can be installed as a standalone app
- 🎨 **Color-coded subjects** - Different colors for different class types:
  - **Theory** (Blue) - Theoretical lectures
  - **Elective** (Yellow) - Elective sessions
  - **Project** (Red) - Project work
  - **Free** (Orange) - Free periods
  - **Tutorial** (Purple) - Tutorial sessions
  - **Others** (Green) - Special Class and Lab Periods
- ⏱️ **Time tracking** - Shows current time and highlights the active class
- 📱 **Responsive design** - Optimized for mobile and tablet devices
- 🚀 **Fast loading** - Service worker enables offline functionality

## Project Structure

```
timetable/
├── index.html      # Main application UI
├── manifest.json   # PWA manifest configuration
├── sw.js          # Service worker for offline support
└── README.md      # This file
```

## Files

- **index.html** - Contains the complete UI with embedded styles and timetable data
- **manifest.json** - PWA manifest for app installation and metadata
- **sw.js** - Service worker for caching and offline support

## Installation

### As a Web App
1. Open `index.html` in a modern web browser
2. Click the install button (usually in the address bar) to add to home screen
3. Or visit the URL and access as a standalone app

### Local Development
Simply open `index.html` directly in your browser or serve via a local web server:
```bash
# Using Python
python -m http.server 8000

# Using Node.js (http-server)
npx http-server
```

Then navigate to `http://localhost:8000`

## Browser Support

- Chrome/Edge 45+
- Firefox 39+
- Safari 11.1+
- Opera 32+

## Offline Support

The service worker automatically caches the app on first load. Subsequently, the app works completely offline.

## Customization

Edit the timetable data in `index.html` by modifying the classes array in the JavaScript section to add or change your schedule.

## License

This project is open source and available under the MIT License.
