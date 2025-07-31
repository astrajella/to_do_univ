# To-Do Universe 🌌

A cosmic task management application where your tasks float in 3D space. Built as a single HTML file with WebGL graphics, smooth animations, and a space-themed interface.

## ✨ Features

### 🎮 Core Functionality
- **3D Task Positioning**: Tasks exist in 3D space with x, y, z coordinates
- **Interactive Cards**: Hover effects, scaling, and neon glow
- **Context Menus**: Right-click/long-press for edit, duplicate, follow, delete
- **Modal Editing**: Inline task editing with form validation
- **Priority System**: High, medium, low priority with color coding

### 🎨 Visual Design
- **Neon Color Scheme**: Each task gets a random neon color with proper contrast
- **Space Theme**: Dark background with cosmic aesthetics
- **Responsive Design**: Works on desktop and mobile devices
- **Smooth Animations**: 60fps rendering with CSS transitions

### 🛠️ Advanced Features
- **Radar System**: Top-left minimap showing task positions and camera
- **System Messages**: Bottom-left ticker with typewriter effect
- **Side Menu**: Hidden menu with save, export, import, orbit mode
- **Keyboard Shortcuts**: 1/2/3 for priority filtering, WASD for camera
- **Local Storage**: Persistent state management
- **Export/Import**: JSON data exchange

### 📱 Mobile Support
- **Touch Gestures**: Pinch-to-zoom, swipe, long-press
- **Responsive Breakpoints**: 600px and 1024px media queries
- **Mobile-Optimized UI**: Smaller radar, adjusted card sizes

## 🚀 Quick Start

1. **Download**: Save `todo-universe.html` to your computer
2. **Open**: Double-click the file to open in any modern browser
3. **Start**: The app will load with sample tasks to get you started

## 🎯 How to Use

### Basic Operations
- **Add Task**: Double-click empty space or use context menu
- **Edit Task**: Double-click any task card
- **Move Camera**: Drag to pan, scroll to zoom, use WASD keys
- **Filter Tasks**: Press 1/2/3 for priority filtering

### Advanced Features
- **Export Data**: Hover right edge → Export JSON
- **Import Data**: Hover right edge → Import JSON
- **Save State**: Automatically saves to localStorage
- **Reset Camera**: Hover right edge → Reset Camera

### Keyboard Shortcuts
- `1` - Filter high priority tasks
- `2` - Filter medium priority tasks  
- `3` - Filter low priority tasks
- `W/A/S/D` - Move camera
- `ESC` - Close modal
- `Mouse Wheel` - Zoom in/out

## 🏗️ Technical Details

### Architecture
- **Pure Frontend**: No server required, runs entirely in browser
- **ES6+ JavaScript**: Modern classes, modules, async/await
- **CSS Grid/Flexbox**: Responsive layout system
- **Canvas API**: 2D radar system
- **LocalStorage**: Client-side data persistence

### Performance
- **60fps Rendering**: Optimized animation loops
- **Debounced Events**: Resize and orientation change handling
- **Memory Management**: Efficient task rendering and cleanup
- **Mobile Optimized**: Touch-friendly interactions

### Browser Support
- **Modern Browsers**: Chrome, Firefox, Safari, Edge
- **Mobile Browsers**: iOS Safari, Chrome Mobile
- **Fallbacks**: Graceful degradation for older browsers

## 📊 Data Model

Each task contains:
```javascript
{
  id: "uuid-v4",
  title: "Task Title",
  brief: "Description",
  links: ["url1", "url2"],
  tags: ["tag1", "tag2"],
  priority: "high|medium|low",
  coords: { x: 0, y: 0, z: 0 },
  color: "#RRGGBB",
  createdAt: Date,
  updatedAt: Date
}
```

## 🔧 Customization

### Colors
The app uses HSL color generation for neon effects:
- Hue: Random (0-360)
- Saturation: 80-100%
- Lightness: 50-70%

### Styling
All styles are contained in the `<style>` section and can be modified:
- Change fonts in `body` selector
- Adjust colors in `.task-card` classes
- Modify animations in transition properties

## 🐛 Troubleshooting

### Common Issues
1. **App won't load**: Check browser console for errors
2. **Tasks not saving**: Ensure localStorage is enabled
3. **Performance issues**: Close other tabs, restart browser
4. **Touch not working**: Try refreshing the page

### Browser Compatibility
- **WebGL**: Required for 3D features (fallback available)
- **LocalStorage**: Required for data persistence
- **Canvas API**: Required for radar system

## 📝 License

This project is open source and available under the MIT License.

## 🤝 Contributing

Feel free to fork this project and submit pull requests for improvements!

## 🌟 Credits

Created as a demonstration of modern web technologies and creative UI/UX design. The space theme and cosmic aesthetics make task management an immersive experience.

---

**Enjoy managing your tasks in the cosmic void! 🌌✨**