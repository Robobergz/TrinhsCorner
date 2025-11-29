# Vietnamese Restaurant Menu Website

A mobile-friendly, responsive restaurant menu website for displaying your Vietnamese cuisine offerings.

## 🚀 Quick Start

1. Clone this repository or download the files
2. Open `index.html` in any web browser
3. The site works offline - no server required!

## 📁 File Structure

```
restaurant-menu-site/
├── index.html              # Main menu website
├── assets/
│   └── images/            # Place your food images here
│       ├── header-image.png
│       ├── pho/           # Pho images (optional organization)
│       ├── banh-mi/       # Banh Mi images
│       ├── drinks/        # Drink images
│       └── appetizers/    # Appetizer images
├── README.md              # This file
└── IMAGES-GUIDE.md        # Guide for adding your own images
```

## 🖼️ Adding Your Own Images

### Current Placeholders
The menu currently uses colorful gradient placeholders with emojis. To replace them with your actual food photos:

### Step 1: Prepare Your Images
- **Recommended size**: 800px x 600px (4:3 ratio)
- **Format**: JPG or PNG
- **File size**: Keep under 500KB per image for fast loading

### Step 2: Name Your Images
Use descriptive names that match your menu items:

**Pho Items:**
- `pho-house-special.jpg`
- `pho-rare-steak.jpg`
- `pho-brisket.jpg`
- `pho-meatball.jpg`
- `pho-beef-ribs.jpg`
- `pho-chicken.jpg`

**Banh Mi Items:**
- `banh-mi-beef.jpg`
- `banh-mi-pork.jpg`
- `banh-mi-chicken.jpg`
- `banh-mi-eggs.jpg`

**Spring Rolls:**
- `spring-roll-shrimp.jpg`
- `spring-roll-tofu.jpg`

**Other Items:**
- `eggrolls.jpg`
- `vermicelli-pork.jpg`
- `vermicelli-chicken.jpg`
- `vermicelli-beef.jpg`
- etc.

### Step 3: Place Images in assets/images/
Drop all your images into the `assets/images/` folder.

### Step 4: Update HTML
Open `index.html` and replace the placeholder divs with image tags:

**Find lines like:**
```html
<div class="item-image-placeholder pho-bg">🍜</div>
```

**Replace with:**
```html
<img src="assets/images/pho-house-special.jpg" alt="Pho House Special" class="item-image">
```

Do this for each menu item you have photos for.

## 🎨 Customization

### Colors
Edit the CSS variables in `index.html` (around line 13):
```css
:root {
    --primary-color: #d4462c;      /* Main red color */
    --secondary-color: #f8f5f0;    /* Background beige */
    --accent-gold: #d4a574;        /* Gold accent */
}
```

### Menu Items
Edit the HTML content directly in `index.html` to:
- Update prices
- Add/remove items
- Change descriptions
- Modify Vietnamese translations

### Header Image
Replace `assets/images/header-image.png` with your own banner image.

## 📱 Features

✅ **Mobile-First Design** - Optimized for phones and tablets  
✅ **Category Navigation** - Easy tabs for Home, Appetizers, and Drinks  
✅ **Size Options** - Supports Regular/Large sizing for soups and sandwiches  
✅ **Touch-Friendly** - Smooth animations and interactions  
✅ **No Dependencies** - Pure HTML/CSS/JavaScript, works anywhere  
✅ **Offline Ready** - No internet required once loaded  

## 🌐 Deployment Options

### GitHub Pages (Free Hosting)
1. Push this code to a GitHub repository
2. Go to Settings → Pages
3. Select main branch as source
4. Your site will be live at `https://yourusername.github.io/repository-name`

### Netlify (Free Hosting)
1. Drag and drop the entire folder to [netlify.com/drop](https://netlify.com/drop)
2. Get an instant live URL

### Vercel (Free Hosting)
1. Push to GitHub
2. Import project at [vercel.com](https://vercel.com)
3. Deploy with one click

## 📝 License

Free to use and modify for your restaurant.

## 🆘 Support

For questions or issues, refer to `IMAGES-GUIDE.md` for detailed image replacement instructions.

---

Made with ❤️ for Vietnamese Cuisine
