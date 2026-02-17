# Product Comparison Section - Shopify Liquid

A pixel-perfect recreation of the "How Q-Rejuvalight compares" section from qureskincare.com as a Shopify section.

Tools Used

1. Cursor
2. OpenCode
3. Kimi K2.5

## 📁 Files to Upload

```
├── assets/
│   ├── Canela-Medium.woff2          # Canela font
│   ├── TTCommons-Regular.woff2      # TT Commons font
│   ├── TTCommons-Medium.woff2       # TT Commons font
│   ├── TTCommons-DemiBold.woff2     # TT Commons font
│   ├── TTCommons-Bold.woff2         # TT Commons font
│   ├── qure-mask.webp               # Product image 1
│   ├── omnilux-mask.webp            # Product image 2
│   ├── dr-dennis-mask.webp          # Product image 3
│   ├── qure-logo.svg                # Brand logo 1
│   ├── omnilux-logo.png             # Brand logo 2
│   └── dr-dennis-logo.svg           # Brand logo 3
└── sections/
    └── product-comparison.liquid    # Main section file
```

## 🚀 Installation

1. Upload all font and image files to your theme's `assets/` folder
2. Copy `product-comparison.liquid` to your theme's `sections/` folder
3. Add the section via Shopify theme editor

## ✨ Features

### Layout
- Row-based flexbox layout (labels left, products right)
- Qure column has mint green background (#D1FAE5)
- Product images positioned above content with negative margin
- Font Awesome-style inline SVG icons

### Responsive Breakpoints
- **Desktop (≥1200px):** 3 products, no slider
- **Tablet (600-1199px):** 2 products with slider
- **Mobile (<600px):** 1 product with slider

### Typography
- **Headings:** Canela Light (serif)
- **Body:** TT Commons (sans-serif)
- Fonts loaded from local theme assets using `asset_url` filter

## 🎨 Customization

### Section Settings
- **Title:** Main heading
- **Footer Text:** Disclaimer at bottom

### Blocks

**Feature Row:**
- `Label`: Feature name (e.g., "Treatment Time")
- `Highlight`: Orange color for important rows

**Product Column:**
- `Featured`: Green background highlight
- `Product Image`: Product photo
- `Brand Logo`: Company logo
- `Product Name`: Title under logo
- `Features`: Format as `check: text` or `cross: text`

## 📐 Technical Details

- Flexbox row layout with `align-items: flex-end`
- Pure JavaScript slider (no dependencies)
- Touch/swipe gesture support
- Inline SVG icons (no external libraries)
- Local font files with `asset_url` filter

## 🎯 Key Measurements

- Label column: 220px (desktop), 120px (mobile)
- Product header: 277px (desktop), 200px (mobile)
- Image height: 150px (normal), 190px (featured)
- Green background: #D1FAE5
- Border color: #DFE0E0

## 📝 Notes

Assets extracted from:
- https://qureskincare.com/products/q-rejuvalight-pro-facewear

Based on live site structure using row-based flexbox layout.
