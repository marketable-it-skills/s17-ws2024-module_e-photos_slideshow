# How to develop and deploy the project?

1. Create a new GitHub repository using the [HTML and Vanilla JS template](https://github.com/new?template_name=mits-html-and-vanila-js-v1&template_owner=marketable-it-skills).
2. Place your solution code inside the `/src` folder.
3. Pushing to GitHub triggers GitHub Actions (see `.github/`) to:
   - Build a Docker image
   - Push it to GitHub Container Registry
4. In `docker-compose.yml`, update:
   `image: ghcr.io/<your-github-account>/<your-repo-name>:latest`
5. Run locally:
   ```bash
   docker compose up -d
   ```
6. Visit: [http://localhost](http://localhost)

## Development Setup

### Prerequisites

- Text editor or IDE (VS Code recommended)
- Modern web browser with developer tools (Chrome, Firefox, Safari, Edge)
- Basic web server for local development (Live Server extension, Python HTTP server, etc.)
- Basic understanding of HTML, CSS, JavaScript, and Web APIs

### Getting Started

1. Navigate to the provided project folder
2. Set up a local web server:
   ```bash
   # Option 1: Using Python (if installed)
   python -m http.server 8000
   
   # Option 2: Using Node.js http-server (if installed)
   npx http-server -p 8000
   
   # Option 3: Using VS Code Live Server extension
   ```
3. Create your slideshow application structure in the `/src` folder
4. Review the provided assets in `/assets/` folder:
   - Sample photos for testing
   - Demo videos showing expected theme behaviors
   - Setting icon for configuration panel
5. Test with the provided sample photos initially
6. Reference the theme demo videos for animation requirements

### Development Guidelines

#### Frontend Architecture
- Build a client-side web application using vanilla HTML, CSS, and JavaScript
- Implement modular CSS structure with separate files for each theme
- Use modern JavaScript features (ES6+, Web APIs)
- Ensure responsive design for different screen sizes
- Implement proper error handling for file operations

#### Core Features Implementation
- **File Loading**: Implement drag-and-drop functionality using File API
- **Photo Management**: Handle file validation, preview generation, and ordering
- **Slideshow Modes**: Manual (keyboard), auto-playing, and random modes
- **Theme System**: Modular CSS themes (A through F) with smooth transitions
- **Command Bar**: Keyboard-activated command interface (Ctrl+K or "/")
- **Fullscreen Mode**: Browser fullscreen API integration

#### Theme Development
- **Theme A**: Direct display without effects
- **Theme B**: Left-to-right sliding with caption delay
- **Theme C**: Bottom-to-top movement with word-by-word caption animation
- **Theme D**: Stack effect with random rotation and photo borders
- **Theme E**: 3D door opening effect with perspective transforms
- **Theme F**: Custom theme with creative animations (student design)

#### User Interface Requirements
- Intuitive drag-and-drop area for photo loading
- Configuration panel for mode and theme switching
- Photo ordering interface with drag-and-drop
- Keyboard navigation support
- Command bar with search and selection functionality
- Fullscreen toggle capability

### Testing and Validation

#### Functionality Testing
- Test drag-and-drop with various image formats (JPG, PNG, GIF)
- Verify all slideshow modes work correctly (manual, auto, random)
- Test all themes (A-F) with proper animations and transitions
- Validate command bar functionality with keyboard navigation
- Test fullscreen mode across different browsers
- Verify photo ordering and caption generation from filenames

#### Cross-Browser Testing
- Test in Firefox Developer Edition and Google Chrome (primary assessment browsers)
- Verify CSS animations work consistently across browsers
- Test Web API compatibility (File API, Fullscreen API)
- Ensure keyboard event handling works properly
- Validate responsive behavior on different screen sizes

#### Performance Considerations
- Optimize image loading and display
- Ensure smooth animations without performance issues
- Test with multiple large images
- Verify memory management with extensive photo sets
- Test CSS transitions and transforms performance

### Code Organization

#### File Structure
```
src/
├── index.html          # Main application file
├── styles/
│   ├── main.css       # Base styles
│   ├── theme-a.css    # Theme A styles
│   ├── theme-b.css    # Theme B styles
│   ├── theme-c.css    # Theme C styles
│   ├── theme-d.css    # Theme D styles
│   ├── theme-e.css    # Theme E styles
│   └── theme-f.css    # Theme F styles (custom)
├── scripts/
│   ├── main.js        # Core application logic
│   ├── slideshow.js   # Slideshow functionality
│   ├── themes.js      # Theme management
│   └── commandbar.js  # Command bar implementation
└── assets/            # Static assets
```

#### Best Practices
- Use semantic HTML structure
- Implement CSS custom properties for theme consistency
- Write modular, reusable JavaScript functions
- Follow accessibility guidelines where applicable
- Comment code thoroughly for maintenance
- Use consistent naming conventions throughout