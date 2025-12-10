# LinkBase 🔗

A modern, fully customizable "link in bio" page that you can host anywhere. Perfect for social media profiles, business cards, or as a personal landing page.

## ✨ Features

- **Fully Customizable** - Edit a simple JSON file to update all content
- **Modern Design** - Beautiful gradient backgrounds and smooth animations
- **Responsive** - Works perfectly on mobile, tablet, and desktop
- **Fast & Lightweight** - No frameworks or dependencies
- **Easy to Deploy** - Host on GitHub Pages, Netlify, Vercel, or any static host
- **Social Media Icons** - Pre-built icons for all major platforms
- **Theme Support** - Customize colors and gradients

## 🚀 Quick Start

### 1. Clone or Download

```bash
git clone https://github.com/AkideweKuseh/LinkBase.git
cd LinkBase
```

### 2. Customize Your Page

Edit `config.json` to add your information:

```json
{
  "profile": {
    "name": "Your Name",
    "bio": "Your bio here",
    "avatar": "assets/images/avatar-placeholder.svg"
  },
  "theme": {
    "backgroundGradient": "linear-gradient(135deg, #667eea 0%, #764ba2 100%)",
    "primaryColor": "#667eea"
  },
  "links": [
    {
      "title": "My Website",
      "url": "https://yourwebsite.com",
      "icon": "🌐",
      "enabled": true
    }
  ],
  "socialLinks": [
    {
      "platform": "github",
      "url": "https://github.com/yourusername",
      "enabled": true
    }
  ]
}
```

### 3. Add Your Avatar

Replace `assets/images/avatar-placeholder.svg` with your own image, or update the path in `config.json`.

### 4. Open in Browser

Simply open `index.html` in your web browser to preview your page locally.

## 📝 Configuration Guide

### Profile Section

```json
"profile": {
  "name": "Your Name",           // Your display name
  "bio": "Your bio description", // Short bio (1-2 sentences)
  "avatar": "path/to/image.jpg"  // Path to your profile image
}
```

### Theme Customization

```json
"theme": {
  "backgroundGradient": "linear-gradient(135deg, #667eea 0%, #764ba2 100%)",
  "primaryColor": "#667eea"
}
```

**Popular Gradient Examples:**

- Purple: `linear-gradient(135deg, #667eea 0%, #764ba2 100%)`
- Ocean: `linear-gradient(135deg, #00d2ff 0%, #3a7bd5 100%)`
- Sunset: `linear-gradient(135deg, #fa709a 0%, #fee140 100%)`
- Forest: `linear-gradient(135deg, #0cebeb 0%, #20e3b2 100%)`
- Fire: `linear-gradient(135deg, #f093fb 0%, #f5576c 100%)`

### Adding Links

```json
"links": [
  {
    "title": "Link Title",        // Display text
    "url": "https://example.com", // Target URL
    "icon": "🔗",                 // Emoji icon (any emoji)
    "enabled": true               // Set to false to hide
  }
]
```

**Icon Suggestions:**

- Website: 🌐
- Portfolio: 💼
- Blog: 📝
- Shop: 🛍️
- YouTube: 🎥
- Podcast: 🎙️
- Newsletter: 📧
- Download: 📥

### Social Media Links

Supported platforms: `facebook`, `twitter`, `instagram`, `whatsapp`, `tiktok`, `youtube`, `linkedin`, `github`, `email`, `website`

```json
"socialLinks": [
  {
    "platform": "github",              // Platform name (lowercase)
    "url": "https://github.com/user",  // Your profile URL
    "enabled": true                    // Set to false to hide
  }
]
```

## 🌐 Deployment

### GitHub Pages

1. Push your code to a GitHub repository
2. Go to repository Settings → Pages
3. Select "Deploy from a branch"
4. Choose `main` branch and `/root` folder
5. Click Save
6. Your site will be live at `https://yourusername.github.io/LinkBase`

### Netlify

1. Go to [netlify.com](https://netlify.com)
2. Click "Add new site" → "Import an existing project"
3. Connect your GitHub repository
4. Leave build settings empty (static site)
5. Click "Deploy"

### Vercel

1. Go to [vercel.com](https://vercel.com)
2. Click "Add New" → "Project"
3. Import your GitHub repository
4. Click "Deploy"

### Other Hosting

Upload all files to any web hosting service that supports static HTML files.

## 🎨 Customization Tips

### Changing Colors

1. Use a gradient generator like [cssgradient.io](https://cssgradient.io)
2. Copy the CSS gradient code
3. Paste into `theme.backgroundGradient` in `config.json`

### Using Your Own Avatar

- Recommended size: 400x400px or larger
- Supported formats: JPG, PNG, SVG, WebP
- Place image in `assets/images/` folder
- Update path in `config.json`

### Advanced Styling

For advanced customization, edit `assets/css/styles.css`:

- Change fonts
- Adjust button styles
- Modify animations
- Update spacing and layout

## 📁 Project Structure

```
LinkBase/
├── index.html              # Main HTML file
├── config.json            # Configuration file (edit this!)
├── README.md              # Documentation
├── assets/
│   ├── css/
│   │   └── styles.css     # Stylesheet
│   ├── js/
│   │   └── script.js      # JavaScript logic
│   └── images/
│       └── avatar-placeholder.svg  # Default avatar
```

## 🔧 Troubleshooting

**Links not appearing?**

- Check that `enabled: true` is set for each link
- Verify the JSON syntax is correct (no missing commas or brackets)

**Avatar not showing?**

- Verify the image path is correct in `config.json`
- Make sure the image file exists in the specified location

**Page looks broken?**

- Validate your `config.json` at [jsonlint.com](https://jsonlint.com)
- Check browser console for error messages (F12)

**Social icons not working?**

- Verify platform name is lowercase and spelled correctly
- Check that URL is complete (includes https://)

## 🤝 Contributing

Contributions are welcome! Feel free to:

- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

## 📄 License

This project is open source and available under the MIT License.

## 💡 Ideas for Enhancement

- [ ] Dark/Light mode toggle
- [ ] Analytics integration
- [ ] Custom fonts support
- [ ] Image backgrounds
- [ ] Animation customization
- [ ] QR code generator
- [ ] Visitor counter

## 🙋 Support

If you have questions or need help:

- Open an issue on GitHub
- Check existing issues for solutions
- Review the configuration examples

---

**Made with ❤️ by LinkBase**

⭐ Star this repo if you find it useful!
