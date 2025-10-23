# 🎨 Logo Setup Guide

## 📁 **Where to Add Your Logo Files**

### **1. Public Folder Structure**
```
tria-contact-list/
├── public/
│   ├── logo.png          # Main logo (PNG format)
│   ├── logo.svg          # Vector logo (SVG format) - Recommended
│   ├── logo-dark.png     # Dark theme logo
│   ├── logo-light.png    # Light theme logo
│   └── favicon.ico       # Browser tab icon
```

### **2. Logo File Requirements**

#### **Main Logo (logo.png/logo.svg)**
- **Size**: 512x512px minimum
- **Format**: PNG (with transparency) or SVG (recommended)
- **Background**: Transparent
- **Style**: Should work on both light and dark backgrounds

#### **Favicon (favicon.ico)**
- **Size**: 32x32px, 16x16px
- **Format**: ICO format
- **Background**: Transparent or solid

## 🔧 **How to Add Your Logo**

### **Option 1: Image Logo (Easiest)**
1. Add your logo file to `public/logo.png`
2. Update the Logo component:

```tsx
// In src/components/Logo.tsx
<img src="/logo.png" alt="Tria Logo" className="w-3/4 h-3/4 object-contain" />
```

### **Option 2: SVG Logo (Best Quality)**
1. Add your logo file to `public/logo.svg`
2. Update the Logo component:

```tsx
// In src/components/Logo.tsx
<img src="/logo.svg" alt="Tria Logo" className="w-3/4 h-3/4 object-contain" />
```

### **Option 3: Custom SVG Code (Most Control)**
Replace the SVG path in `src/components/Logo.tsx`:

```tsx
<svg className="w-3/4 h-3/4 text-white" viewBox="0 0 24 24" fill="currentColor">
  {/* Replace this path with your logo's SVG path */}
  <path d="YOUR_LOGO_SVG_PATH_HERE"/>
</svg>
```

## 🎨 **Logo Placement Options**

### **1. Header Logo (Current)**
- **Location**: Top-left of the app
- **Size**: Medium (48x48px)
- **Usage**: Main branding

### **2. Favicon**
- **Location**: Browser tab
- **Size**: 16x16px, 32x32px
- **Usage**: Browser identification

### **3. Loading Screen Logo**
- **Location**: App startup
- **Size**: Large (128x128px)
- **Usage**: First impression

### **4. Footer Logo**
- **Location**: Bottom of the app
- **Size**: Small (32x32px)
- **Usage**: Additional branding

## 🚀 **Quick Setup Steps**

1. **Add your logo file** to `public/logo.png`
2. **Update the Logo component** to use your image
3. **Test the logo** in both light and dark modes
4. **Add favicon** for browser tab icon
5. **Customize colors** to match your brand

## 💡 **Logo Design Tips**

- **Keep it simple** - works well at small sizes
- **Use your brand colors** - matches the Tria theme
- **Test on dark backgrounds** - ensure good contrast
- **Make it scalable** - SVG format recommended
- **Consider animation** - subtle hover effects

## 🎯 **Current Logo Implementation**

The app currently uses a placeholder "T" logo with gradient background. To replace it:

1. **Replace the image source** in `Logo.tsx`
2. **Adjust the size** if needed
3. **Test responsiveness** on different screen sizes
4. **Ensure accessibility** with proper alt text

## 📱 **Responsive Logo Sizes**

- **Mobile**: 32x32px
- **Tablet**: 48x48px  
- **Desktop**: 64x64px
- **Large screens**: 80x80px

Your logo will automatically scale based on the `size` prop passed to the Logo component!
