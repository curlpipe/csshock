# CSShock ⚡

If you've ever found CSS cumbersome, try CSShock: a single-file CSS library with simple theming, an easy, powerful and intuitive layout system and tailwind-style utility classes.

## ✨ Features

- **🎯 Single-File Library** - Drop in one CSS file and start building
- **🎨 Simple Theming** - Easy-to-use theming system for consistent designs
- **📐 Powerful Layout System** - Intuitive and flexible layouts without the complexity
- **🚀 Utility Classes** - Tailwind-style utilities for rapid development
- **⚡ Zero Configuration** - No build tools or complicated setup required

## 📦 Installation

### CDN

Add CSShock to your HTML file via CDN:

```html
<link rel="stylesheet" href="https://unpkg.com/csshock@latest/csshock.css">
```

### NPM

Install via npm:

```bash
npm install csshock
```

### Download

Download the `csshock.css` file directly and include it in your project:

```html
<link rel="stylesheet" href="path/to/csshock.css">
```

## 🚀 Quick Start

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSShock Example</title>
    <link rel="stylesheet" href="https://unpkg.com/csshock@latest/csshock.css">
</head>
<body>
    <div class="container">
        <h1>Welcome to CSShock</h1>
        <p>Start building beautiful interfaces with ease!</p>
    </div>
</body>
</html>
```

## 📖 Usage

### Layout System

CSShock provides an intuitive layout system:

```html
<div class="flex justify-center items-center">
    <div class="card">
        <h2>Card Title</h2>
        <p>Card content goes here</p>
    </div>
</div>
```

### Utility Classes

Use tailwind-style utilities for quick styling:

```html
<div class="p-4 m-2 bg-primary text-white rounded">
    Styled with utility classes
</div>
```

### Theming

Apply themes easily with CSShock's theming system:

```css
:root {
    --primary-color: #007bff;
    --secondary-color: #6c757d;
    /* Add more theme variables */
}
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by modern CSS frameworks and utility-first approaches
- Built with ❤️ for developers who want simplicity without sacrificing power

---

**Made with ⚡ by [curlpipe](https://github.com/curlpipe)**
