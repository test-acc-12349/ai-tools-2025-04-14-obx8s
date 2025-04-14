# AI Tools Directory Website 🤖

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Netlify Status](https://api.netlify.com/api/v1/badges/your-badge/deploy-status)](https://app.netlify.com/)

A comprehensive directory website showcasing the latest AI tools and resources in a clean, responsive 3-column grid layout.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Support & Resources](#support--resources)

## Overview

AI Tools is a curated directory website that helps users discover and compare artificial intelligence tools and resources. The website features a responsive design, filtering capabilities, and an easy-to-navigate interface.

## Features

- Responsive 3-column grid layout
- Category-based filtering
- Search functionality
- Sorting options
- Mobile-friendly design
- SEO optimized
- Fast loading times
- Easy customization

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/ai-tools-directory.git

# Navigate to project directory
cd ai-tools-directory

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure

```
ai-tools-directory/
├── src/
│   ├── components/
│   ├── data/
│   │   ├── tools.json
│   │   └── categories.json
│   ├── styles/
│   └── pages/
├── public/
│   └── images/
├── package.json
└── README.md
```

## Customization Guide

### Adding New Directory Items

1. Open `src/data/tools.json`
2. Add new item using the following format:

```json
{
  "id": "unique-id",
  "name": "Tool Name",
  "description": "Tool description",
  "category": "category-slug",
  "url": "https://toolurl.com",
  "image": "/images/tool-image.png"
}
```

### Modifying Categories

1. Navigate to `src/data/categories.json`
2. Edit categories using this structure:

```json
{
  "id": "category-slug",
  "name": "Category Name",
  "description": "Category description"
}
```

### Updating Hero Section

1. Open `src/components/Hero.js`
2. Modify the content:

```jsx
<div className="hero">
  <h1>Your New Title</h1>
  <p>Your new description</p>
</div>
```

### Customizing Colors

1. Edit `src/styles/variables.css`:

```css
:root {
  --primary-color: #your-color;
  --secondary-color: #your-color;
  --background-color: #your-color;
  --text-color: #your-color;
}
```

## Deployment

### Netlify Deployment

1. Push your code to GitHub
2. Login to Netlify
3. Click "New site from Git"
4. Select your repository
5. Configure build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
6. Click "Deploy site"

## Custom Domain Setup

1. Purchase domain from your preferred registrar
2. In Netlify:
   - Go to Site settings > Domain management
   - Click "Add custom domain"
   - Enter your domain name
3. Update DNS settings:
   - Add CNAME record pointing to your Netlify URL
   - Wait for DNS propagation (24-48 hours)

## Troubleshooting

### Common Issues

1. Build Errors
```bash
# Clear cache and node_modules
rm -rf node_modules
rm -rf .cache
npm install
```

2. Image Loading Issues
- Ensure images are in the correct format (PNG/JPG/WebP)
- Verify file paths are correct
- Check image dimensions match requirements

3. Styling Issues
- Clear browser cache
- Verify CSS compilation
- Check browser console for errors

## Support & Resources

- [Documentation Wiki](https://github.com/yourusername/ai-tools-directory/wiki)
- [Issue Tracker](https://github.com/yourusername/ai-tools-directory/issues)
- [Contributing Guidelines](CONTRIBUTING.md)

### Community
- [Discord Server](https://discord.gg/your-server)
- [Twitter](https://twitter.com/your-handle)
- Email: support@aitools-directory.com

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Built with ❤️ by [Your Name](https://yourwebsite.com)