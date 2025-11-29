# Image Replacement Guide

This guide will help you replace the placeholder gradients with your actual food photos.

## 📸 Image Specifications

### Recommended Specs
- **Dimensions**: 800px wide × 600px tall (or any 4:3 ratio)
- **Format**: JPG (smaller file size) or PNG (better quality)
- **File Size**: 200-500KB per image
- **Quality**: 80-90% for JPG compression

### Image Optimization Tools
- [TinyPNG](https://tinypng.com) - Compress images online
- [Squoosh](https://squoosh.app) - Google's image optimizer
- [ImageOptim](https://imageoptim.com) - Mac app for compression

## 🗂️ Suggested File Organization

You can organize images in subfolders within `assets/images/`:

```
assets/images/
├── header-image.png
├── pho/
│   ├── house-special.jpg
│   ├── rare-steak.jpg
│   ├── brisket.jpg
│   ├── meatball.jpg
│   ├── beef-ribs.jpg
│   └── chicken.jpg
├── banh-mi/
│   ├── beef.jpg
│   ├── pork.jpg
│   ├── chicken.jpg
│   └── eggs.jpg
├── appetizers/
│   ├── spring-rolls-shrimp.jpg
│   ├── spring-rolls-tofu.jpg
│   ├── eggrolls.jpg
│   ├── chicken-wings.jpg
│   ├── french-fries.jpg
│   ├── popcorn-chicken.jpg
│   └── croffles/
│       ├── tiramisu.jpg
│       ├── choco-berry.jpg
│       ├── oreo-crunch.jpg
│       ├── biscoff.jpg
│       └── purple-cloud.jpg
├── vermicelli/
│   ├── pork.jpg
│   ├── chicken.jpg
│   └── beef.jpg
├── rice/
│   ├── pork-egg.jpg
│   ├── chicken-egg.jpg
│   └── beef-ribs.jpg
└── drinks/
    ├── coffee/
    │   ├── saigon.jpg
    │   ├── marble-drip.jpg
    │   └── etc.jpg
    ├── milk-tea/
    ├── matcha/
    ├── fruit-tea/
    ├── soda/
    └── smoothies/
```

## 🔧 How to Replace Placeholders

### Step-by-Step Process

#### 1. Find the Placeholder Code

Open `index.html` and search for sections like this:

```html
<div class="menu-item">
    <div class="item-image-placeholder pho-bg">🍜</div>
    <div class="item-content">
        <div class="item-header">
            <span class="item-code">P01</span>
            <span class="item-name">House Special</span>
        </div>
        ...
    </div>
</div>
```

#### 2. Replace with Image Tag

Change the `<div class="item-image-placeholder...">` line to:

```html
<img src="assets/images/pho/house-special.jpg" alt="Pho House Special" class="item-image">
```

#### 3. Complete Example

**BEFORE:**
```html
<div class="menu-item">
    <div class="item-image-placeholder pho-bg">🍜</div>
    <div class="item-content">
```

**AFTER:**
```html
<div class="menu-item">
    <img src="assets/images/pho/house-special.jpg" alt="Pho House Special" class="item-image">
    <div class="item-content">
```

## 📋 Complete Item List

Here's a complete list of all menu items that need images:

### Pho (6 items)
- P01: House Special
- P02: Rare Steak
- P03: Brisket
- P04: Meatball
- P05: Beef Ribs
- P06: Chicken

### Banh Mi (4 items)
- M01: Grilled Beef
- M02: Grilled Pork
- M03: Grilled Chicken
- M04: Sunny Side Up Eggs

### Spring Rolls (2 items)
- G01: Shrimp
- G02: Tofu

### Eggrolls (1 item)
- B04: Eggrolls Only

### Vermicelli Bowls (3 items)
- B01: Grilled Lemongrass Pork
- B02: Grilled Lemongrass Chicken
- B03: Grilled Lemongrass Beef

### Rice Combos (3 items)
- R01: Grilled Pork w/ Egg
- R02: Grilled Chicken w/ Egg
- R03: Grilled Beef Short Ribs

### Coffee (7 items)
- C01-C07: Various coffee drinks

### Milk Tea (5 items)
- M01-M05: Various milk tea drinks

### Matcha Lattes (3 items)
- L01-L03: Matcha variations

### Fruit Teas (6 items)
- F01-F06: Various fruit teas

### Sodas (6 items)
- S01-S06: Various sodas

### Smoothies (4 items)
- I01-I04: Various smoothies

### Appetizers
- Chicken Wings
- French Fries
- Popcorn Chicken

### Croffles (5 items)
- Tiramisu Delight
- Choco Berry
- Oreo Crunch
- Biscoff
- Purple Cloud

**Total: ~58 images needed**

## 💡 Pro Tips

### Don't Have All Images Yet?
You can replace images gradually. The placeholders will remain for items without photos.

### Use Consistent Styling
- Take photos with similar lighting
- Use the same background/plate style
- Maintain consistent angles (top-down or 45-degree angle works best)

### Alt Text Matters
Always include descriptive alt text for accessibility:
```html
<img src="..." alt="Steaming bowl of Pho with rare steak and fresh herbs" class="item-image">
```

### Test After Adding Images
1. Save your changes to `index.html`
2. Refresh the browser
3. Check that images load correctly
4. Verify they look good on mobile (resize browser window)

## 🔄 Batch Replace (Advanced)

If you're comfortable with code editors like VS Code:

1. Use Find & Replace (Ctrl/Cmd + H)
2. Find: `<div class="item-image-placeholder pho-bg">🍜</div>`
3. Replace: `<img src="assets/images/pho/ITEM-NAME.jpg" alt="DESCRIPTION" class="item-image">`
4. Do this for each category

## ✅ Checklist

- [ ] Images prepared and optimized
- [ ] Images placed in `assets/images/` folder
- [ ] Placeholders replaced with `<img>` tags in HTML
- [ ] Image paths are correct
- [ ] Alt text added for all images
- [ ] Tested in browser
- [ ] Tested on mobile device
- [ ] Committed changes to Git
- [ ] Pushed to GitHub

## 🆘 Troubleshooting

**Images not showing?**
- Check file path spelling (case-sensitive!)
- Verify image files are in correct folder
- Check browser console for errors (F12)

**Images too large/slow?**
- Optimize images with TinyPNG or Squoosh
- Target 200-500KB per image

**Images look stretched?**
- Use 4:3 aspect ratio (800×600px)
- The CSS will crop them to fit perfectly

---

Need more help? Check the main README.md file.
