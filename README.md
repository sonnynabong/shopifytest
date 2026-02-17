# Product Comparison Section - Exact Match to Qure Live Site

A pixel-perfect recreation of the "How Q-Rejuvalight compares" section from qureskincare.com.

## 📁 Project Structure

```
shopifytest/
├── assets/
│   ├── comparison-section.css    # Exact match styles
│   ├── qure-mask.webp            # Product image 1
│   ├── omnilux-mask.webp         # Product image 2  
│   ├── dr-dennis-mask.webp       # Product image 3
│   ├── qure-logo.svg             # Brand logo 1
│   ├── omnilux-logo.svg          # Brand logo 2
│   └── dr-dennis-logo.svg        # Brand logo 3
├── sections/
│   └── product-comparison.liquid # Shopify section
├── index.html                     # Standalone version (inline styles)
├── comparison-section.html        # Modular version (external CSS)
└── reference/
    ├── desktop.png                # Desktop reference
    └── mobile.png                 # Mobile reference
```

## 🚀 Quick Start

### Option 1: View Standalone
Open `index.html` in your browser to see the exact replica.

### Option 2: Shopify Integration
1. Copy `sections/product-comparison.liquid` to your theme's `sections/` folder
2. Copy all files from `assets/` to your theme's `assets/` folder
3. Add the section in Shopify theme editor

## ✨ Exact Features from Live Site

### Layout Structure
- **Row-based flexbox layout** (not column-based)
- Left side: Feature labels (220px desktop, 120px mobile)
- Right side: Product columns in flex row
- Qure column has mint green background extending full height

### Desktop (>768px)
- 4-column layout: 1 label column + 3 product columns
- Product images positioned above with negative margin
- Featured (Qure) box has green background (#D1FAE5)
- Check icons are green for featured product, grey for others
- Cross icons are grey for all
- Orange highlighted "Wavelengths" row

### Mobile (≤768px)  
- Left labels column: 120px width
- Right products: Slider/carousel showing 1 product at a time
- Previous/Next navigation buttons
- Slide counter (1/3, 2/3, 3/3)
- Touch/swipe gesture support

### Icons
- Uses inline SVG (Font Awesome style) instead of external library
- Check circle: Green (#008763) for featured, grey (#8b8c8e) for others
- Cross circle: Grey for all products

### Typography
- Title: Georgia serif font
- Product names: Georgia serif, 22px
- Labels: Inter sans-serif, 16px, font-weight 600
- Items: Inter sans-serif, 14px

## 🎨 Customization (Shopify)

### Section Settings
- **Title**: Main heading
- **Footer Text**: Disclaimer at bottom

### Feature Row Blocks
- **Label**: Feature name (e.g., "Treatment Time")
- **Highlight**: Orange color for important rows

### Product Column Blocks  
- **Featured**: Green background highlight
- **Product Image**: Product photo
- **Brand Logo**: Company logo
- **Product Name**: Title under logo
- **Features**: Format as `type: text`
  - `check: Feature description` (shows green checkmark)
  - `cross: Feature description` (shows grey X)

## 📐 Technical Details

### CSS Architecture
- Flexbox row layout: `display: flex; align-items: flex-end`
- CSS custom properties for heights
- Negative margins for overlapping images
- Mobile slider with CSS transform

### Key Measurements (from live site)
- Label column: 220px (desktop), 120px (mobile)
- Product header height: 277px (desktop), 200px (mobile)
- Content area height: 390px total / 5 items = 78px per item
- Item min-height: 66px
- Image height: 150px (normal), 190px (featured)
- Green background: #D1FAE5 (mint)
- Border color: #DFE0E0

### Mobile Slider
- Pure JavaScript (no dependencies)
- CSS transform for smooth sliding
- Touch event support
- Responsive breakpoint at 767px

## 🎯 Exact Match Checklist

- ✅ Row-based layout (labels on left, products on right)
- ✅ Qure column has full-height mint green background
- ✅ Product images positioned above content with overlap
- ✅ Font Awesome-style check/X icons as inline SVG
- ✅ Green checkmarks only on featured product
- ✅ Orange highlight on "Wavelengths" label
- ✅ Mobile slider with nav buttons
- ✅ Touch/swipe support on mobile
- ✅ Exact spacing and measurements from live site

## 📝 Notes

All assets extracted from:
- https://qureskincare.com/products/q-rejuvalight-pro-facewear

CSS extracted from:
- https://qureskincaredns.com/sections/isolated/serum-compare/section-serum-compare.css

Structure matches the live site's implementation using:
- Flexbox row layout
- CSS custom properties (--eq__height, --cp__height)
- Swiper-style mobile slider (recreated in vanilla JS)
