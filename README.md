#Nyanjui Restaurant Website

A responsive restaurant website built with Webpack and JavaScript that features tabbed browsing for different sections.

## Overview

This project creates a modern restaurant website with a dynamic tabbed interface for navigating between pages (Home, Menu, Contact). The site is built entirely with vanilla JavaScript and styled with CSS to create a visually appealing experience.

## Features

- **Responsive Design**: Looks great on desktop and mobile devices
- **Tabbed Navigation**: Switch between different sections without page reloads
- **Dynamic Content Loading**: Content is generated via JavaScript modules
- **Custom Styling**: Themed with restaurant-specific colors
- **Interactive Menu**: Detailed food menu with images, descriptions and prices in KShs
- **Contact Form**: Easy-to-use contact form for customer inquiries

## Screenshots

(Screenshots would be added here once the project is deployed)

## Color Scheme

The website uses the following color palette:
- Primary: #991135
- Secondary: #6c4519
- Accent: #ddac6a
- Dark: #6f0d24
- Light: #fff8e6

## Project Structure

```
restaurant-website/
├── dist/                      # Generated files (created by webpack)
├── src/                       # Source files
│   ├── styles/                # CSS files
│   │   └── style.css         # Main CSS file
│   ├── components/           # JavaScript modules for page components
│   │   ├── home.js          # Home page content
│   │   ├── menu.js          # Menu page content
│   │   └── contact.js       # Contact page content  
│   ├── template.html        # HTML template
│   └── index.js             # Main JavaScript file
├── package.json              # Project configuration
├── webpack.config.js         # Webpack configuration
└── .gitignore                # Git ignore file
```

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm (v6 or higher)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/restaurant-website.git
cd restaurant-website
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

4. Open your browser and navigate to:
```
http://localhost:8080
```

### Building for Production

To create a production build:
```bash
npm run build
```

The build files will be placed in the `dist` directory, ready for deployment to a web server.

## Dependencies

- webpack: Module bundler
- webpack-cli: Command line interface for webpack
- webpack-dev-server: Development server
- html-webpack-plugin: Simplifies creation of HTML files to serve bundles
- style-loader & css-loader: Handle CSS files
- file-loader: Handles file imports

## Customization

### Changing Colors

To update the color scheme, modify the CSS variables in `src/styles/style.css`:

```css
:root {
    --primary: #991135;
    --secondary: #6c4519;
    --accent: #ddac6a;
    --dark: #6f0d24;
    --light: #fff8e6;
}
```

### Adding Menu Items

To add new menu items, edit the `menuItems` array in `src/components/menu.js`.

### Updating Restaurant Information

Restaurant details can be modified in the respective component files:
- General info: `src/components/home.js`
- Menu items: `src/components/menu.js`
- Contact info: `src/components/contact.js`

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Background image from Pinterest
- Inspired by typical restaurant websites
- Created following the Odin Project curriculum
