# Animated Projector Application

A interactive, animated vintage film projector simulation built with HTML, CSS, and JavaScript. This web application creates a realistic projector experience with animated components, multiple film types, and interactive controls.

![Projector Demo](https://img.shields.io/badge/Projector-Animated-ff6b6b)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

##  Features

###  Projector Components
- **Rotating Lens** with dynamic color-changing effects
- **Spinning Film Reels** with realistic animation
- **Moving Film Strip** displaying various pattern frames
- **Flickering Light Beam** for authentic projection feel
- **Vintage-style Projector Body** with metallic finish
- **Projection Screen** with animated geometric patterns

###  Interactive Controls
- **Start/Stop** projection with visual feedback
- **Change Film** to switch between different pattern types
- **Speed Control** slider to adjust animation velocity
- **Status Indicator** showing current projector state
- **Keyboard Shortcuts** for quick control

### Multiple Film Patterns
- **Geometric Patterns** (circles, squares, triangles)
- **Stripes** (horizontal, vertical, diagonal)
- **Gradients** (radial, linear, conic)
- **Abstract Designs** (waves, dots, grids)
- **Color Transitions** (smooth color changes)
- **Motion Patterns** (moving shapes)

###  Visual Effects
- Smooth CSS animations and transitions
- Gradient backgrounds and metallic effects
- Glow effects and shadows for depth
- 3D-like button interactions
- Real-time pattern changes

##  Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/animated-projector.git
   ```

2. **Navigate to project directory**
   ```bash
   cd animated-projector
   ```

3. **Open in browser**
   - Simply open `index.html` in any modern web browser
   - Or use a local server:
     ```bash
     python -m http.server 8000
     ```
     Then visit `http://localhost:8000`

##  Usage

### Mouse Controls
- **START** - Begin projection animation
- **STOP** - Pause projection
- **CHANGE FILM** - Cycle through different pattern types
- **SPEED SLIDER** - Adjust animation speed (0.5x to 3x)
- **Hover over projector** - Speeds up reel animation temporarily

### Keyboard Shortcuts
- **SPACE** - Toggle Start/Stop
- **F** - Change film pattern
- **↑ / ↓** - Increase/Decrease speed
- **R** - Reset to default settings

### Interactive Elements
- Click buttons for visual feedback
- Watch the lens change colors automatically
- Observe the rotating reels and moving film strip
- See the projection screen update with different patterns

##  Technologies Used

- **HTML5** - Structure and layout
- **CSS3** - Animations, gradients, and styling
- **JavaScript** - Interactivity and dynamic content
- **Canvas API** - For advanced pattern rendering

##  Project Structure

```
animated-projector/
│
├── index.html          # Main application file
├── README.md          # Project documentation
├── LICENSE            # MIT License
├── styles/
│   └── main.css       # (Optional) Separated styles
├── scripts/
│   └── projector.js   # (Optional) Separated JavaScript
└── assets/
    └── screenshot.png # Application screenshot
```

##  Pattern Types

| Pattern | Description | Preview |
|---------|-------------|---------|
| **Geometric** | Circles, squares, triangles in rotation | 🔴🔵🟢 |
| **Stripes** | Horizontal, vertical, diagonal lines | ||| |||
| **Gradients** | Smooth color transitions | 🌈 |
| **Abstract** | Waves, dots, and grids | • • • |
| **Color Waves** | Flowing color patterns | 🌊 |
| **Motion Blur** | Simulated movement effects | ➡️ |

##  Configuration

### Adding New Patterns
Edit the `patterns` array in the JavaScript section:

```javascript
const patterns = [
    {
        name: 'Your Pattern',
        frames: [
            'background: linear-gradient(45deg, #color1, #color2)',
            // Add more frame styles
        ]
    }
];
```

### Adjusting Animation Parameters

```javascript
// Speed settings
const speedSettings = {
    min: 0.5,  // Minimum speed multiplier
    max: 3.0,  // Maximum speed multiplier
    default: 1.0
};

// Animation intervals
const animationIntervals = {
    projection: 200,  // Projection update interval (ms)
    lens: 3000,       // Lens color change interval (ms)
    reels: 4000       // Reel rotation duration (ms)
};
```

##  Customization Examples

### Custom Color Scheme
```css
:root {
    --primary-color: #e67e22;
    --secondary-color: #d35400;
    --background-dark: #2c3e50;
    --accent-gold: #f1c40f;
    --light-beam: rgba(255, 255, 255, 0.8);
}
```

### Adding New Animation
```css
@keyframes custom-pattern {
    0% { transform: scale(1) rotate(0deg); }
    50% { transform: scale(1.2) rotate(180deg); }
    100% { transform: scale(1) rotate(360deg); }
}
```

##  Key Animations
| Animation | Description | Default Duration |
|-----------|-------------|------------------|
| `lens-rotate` | Lens rotation and scale | 10s |
| `reel-spin` | Film reel rotation | 4s |
| `light-flicker` | Projector light effect | 0.2s |
| `frame-glow` | Film frame pulsing | 2s |
| `pattern-morph` | Pattern transitions | 3s |
| `color-shift` | Color cycling effects | 5s |

## Browser Support

- Chrome (v90+)
- Firefox (v88+)
- Safari (v14+)
- Edge (v90+)
- Opera (v76+)
- Mobile browsers (iOS Safari, Chrome Android)

##  Performance Optimization

- CSS animations use `transform` and `opacity` for smooth performance
- Debounced event handlers for slider controls
- Optimized animation frames
- Minimal DOM manipulations
- Hardware-accelerated animations where possible

##  Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Contribution Guidelines
- Follow existing code style
- Add comments for complex logic
- Test across different browsers
- Update documentation as needed
- Include pattern previews for new additions

##  License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

##  Acknowledgments

- Inspired by vintage film projectors from the golden age of cinema
- CSS animation techniques from the web development community
- Color theory principles for pattern design
- Performance optimization tips from web animation experts


Project Link: [https://github.com/yourusername/animated-projector](https://github.com/yourusername/animated-projector)

### Version 1.1 (Planned)
- [ ] Sound effects simulation
- [ ] More complex patterns
- [ ] Pattern editor interface
- [ ] Save/load presets

### Version 2.0 (Future)
- [ ] WebGL acceleration
- [ ] 3D projector model
- [ ] Real-time pattern generation
- [ ] Social sharing features
- [ ] Mobile app version

##  Known Issues

- Some complex patterns may cause performance issues on mobile devices
- Safari browser may have limited gradient animation support
- Very high speed settings may cause animation stuttering

##  Stats

- **Lines of Code**: ~500
- **CSS Animations**: 15+
- **Pattern Types**: 6
- **Interactive Elements**: 8
- **Browser Support**: 95%+

##  Tips & Tricks
1. **Speed Control**: Use the slider to create slow-motion or fast-forward effects
2. **Pattern Combinations**: Rapidly change patterns for unique transitions
3. **Focus Mode**: Stop the projector to analyze specific patterns
4. **Presentation Mode**: Full-screen the application for better viewing

## Use Cases

- **Education**: Teaching animation principles
- **Entertainment**: Visual relaxation tool
- **Design**: Pattern inspiration source
- **Development**: CSS animation reference
- **Art**: Digital art installation
