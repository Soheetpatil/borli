# Style Guide - Borli Grampanchayat Website

## 🎨 Color Palette

### Primary Colors
```css
--primary: #2563eb        /* Modern Blue */
--primary-light: #60a5fa  /* Light Blue */
--primary-dark: #1e40af   /* Dark Blue */
```

### Secondary Colors
```css
--secondary: #f59e0b      /* Amber */
--secondary-light: #fbbf24 /* Light Amber */
--secondary-dark: #d97706  /* Dark Amber */
```

### Accent Colors
```css
--accent: #10b981         /* Emerald */
--accent-light: #34d399   /* Light Emerald */
--accent-dark: #059669    /* Dark Emerald */
```

### Neutral Colors
```css
--light: #f0f9ff          /* Very Light Blue */
--dark: #1e3a8a           /* Navy Blue */
--text: #1f2937           /* Dark Gray */
--text-light: #6b7280     /* Medium Gray */
--background: #ffffff     /* White */
--white: #ffffff          /* Pure White */
```

## 📐 Spacing System

### Padding/Margin Scale
- **xs**: 8px
- **sm**: 12px
- **md**: 16px
- **lg**: 24px
- **xl**: 32px
- **2xl**: 48px
- **3xl**: 64px
- **4xl**: 80px
- **5xl**: 100px

### Section Spacing
- Desktop: 100px top/bottom
- Tablet: 80px top/bottom
- Mobile: 60px top/bottom

## 🔤 Typography

### Font Families
```css
Primary: 'Inter', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif
Devanagari: 'Noto Sans Devanagari', 'Arial', sans-serif
```

### Font Sizes
- **Hero Title**: 3.5rem (56px)
- **Section Title**: 2.5rem (40px)
- **Card Title**: 1.5rem (24px)
- **Body Large**: 1.1rem (17.6px)
- **Body**: 1rem (16px)
- **Small**: 0.875rem (14px)

### Font Weights
- **Regular**: 400
- **Medium**: 500
- **Semibold**: 600
- **Bold**: 700
- **Extrabold**: 800
- **Black**: 900

### Line Heights
- **Tight**: 1.2
- **Normal**: 1.5
- **Relaxed**: 1.7
- **Loose**: 1.9

## 🎯 Border Radius

### Standard Sizes
```css
--border-radius-sm: 8px
--border-radius: 16px
--border-radius-lg: 20px
--border-radius-xl: 24px
--border-radius-full: 50px (for pills/badges)
```

## 🌊 Shadows

### Elevation System
```css
/* Small */
box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);

/* Medium */
box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);

/* Large */
box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);

/* Extra Large */
box-shadow: 0 30px 60px rgba(0, 0, 0, 0.12);

/* Colored Shadows */
box-shadow: 0 10px 30px rgba(37, 99, 235, 0.3); /* Blue */
box-shadow: 0 10px 30px rgba(245, 158, 11, 0.3); /* Amber */
box-shadow: 0 10px 30px rgba(16, 185, 129, 0.3); /* Emerald */
```

## 🎨 Gradients

### Background Gradients
```css
/* Primary Gradient */
background: linear-gradient(135deg, #2563eb, #3b82f6);

/* Secondary Gradient */
background: linear-gradient(135deg, #f59e0b, #f97316);

/* Accent Gradient */
background: linear-gradient(135deg, #10b981, #34d399);

/* Multi-color Gradient */
background: linear-gradient(90deg, #2563eb, #f59e0b, #10b981);

/* Section Background */
background: linear-gradient(135deg, #f0f9ff 0%, #e0f2fe 50%, #ffffff 100%);
```

### Text Gradients
```css
background: linear-gradient(135deg, #2563eb, #3b82f6, #60a5fa);
-webkit-background-clip: text;
-webkit-text-fill-color: transparent;
background-clip: text;
```

## 💫 Animations

### Transition Timing
```css
--transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
```

### Common Animations
```css
/* Hover Lift */
transform: translateY(-10px);

/* Hover Scale */
transform: scale(1.05);

/* Hover Rotate */
transform: rotate(5deg);

/* Combined */
transform: translateY(-10px) scale(1.05);
```

### Keyframe Animations
```css
/* Float */
@keyframes float {
    0%, 100% { transform: translateY(0px); }
    50% { transform: translateY(-20px); }
}

/* Pulse */
@keyframes pulse {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.05); }
}

/* Shimmer */
@keyframes shimmer {
    0% { background-position: -1000px 0; }
    100% { background-position: 1000px 0; }
}
```

## 🎴 Card Styles

### Standard Card
```css
.card {
    background: linear-gradient(135deg, #ffffff 0%, #f8fafc 100%);
    border-radius: 20px;
    padding: 30px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
    border: 2px solid rgba(37, 99, 235, 0.1);
    transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
}

.card:hover {
    transform: translateY(-10px);
    box-shadow: 0 20px 40px rgba(37, 99, 235, 0.15);
    border-color: #2563eb;
}
```

### Glass Card
```css
.glass-card {
    background: rgba(255, 255, 255, 0.15);
    backdrop-filter: blur(20px);
    border: 2px solid rgba(255, 255, 255, 0.2);
    box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
}
```

## 🔘 Button Styles

### Primary Button
```css
.btn-primary {
    background: linear-gradient(135deg, #2563eb, #3b82f6);
    color: white;
    padding: 14px 35px;
    border-radius: 50px;
    font-weight: 700;
    box-shadow: 0 10px 25px rgba(37, 99, 235, 0.3);
    transition: all 0.4s ease;
}

.btn-primary:hover {
    transform: translateY(-5px) scale(1.05);
    box-shadow: 0 20px 40px rgba(37, 99, 235, 0.4);
}
```

### Outline Button
```css
.btn-outline {
    background: transparent;
    border: 2px solid #2563eb;
    color: #2563eb;
    padding: 12px 28px;
    border-radius: 50px;
    font-weight: 700;
}

.btn-outline:hover {
    background: #2563eb;
    color: white;
    transform: translateY(-5px);
}
```

## 📱 Responsive Breakpoints

```css
/* Extra Small Devices */
@media (max-width: 576px) { }

/* Small Devices */
@media (max-width: 768px) { }

/* Medium Devices */
@media (max-width: 992px) { }

/* Large Devices */
@media (max-width: 1200px) { }

/* Extra Large Devices */
@media (max-width: 1400px) { }
```

## ✨ Special Effects

### Backdrop Blur
```css
backdrop-filter: blur(20px);
```

### Glass Morphism
```css
background: rgba(255, 255, 255, 0.1);
backdrop-filter: blur(20px);
border: 1px solid rgba(255, 255, 255, 0.2);
box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
```

### Neumorphism
```css
background: #f0f9ff;
box-shadow: 
    8px 8px 16px rgba(37, 99, 235, 0.1),
    -8px -8px 16px rgba(255, 255, 255, 0.9);
```

### Gradient Border
```css
.gradient-border::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    height: 5px;
    background: linear-gradient(90deg, #2563eb, #f59e0b, #10b981);
}
```

## 🎯 Usage Guidelines

### Do's ✅
- Use consistent spacing from the spacing system
- Apply smooth transitions to interactive elements
- Use gradient backgrounds for visual interest
- Maintain proper contrast ratios for accessibility
- Use modern border radius values (16px+)
- Apply shadows for depth and hierarchy
- Use backdrop blur for modern glass effects

### Don'ts ❌
- Don't use flat colors without gradients
- Don't skip hover states on interactive elements
- Don't use small border radius (< 8px)
- Don't forget mobile responsiveness
- Don't use harsh shadows
- Don't mix too many different animation styles
- Don't ignore accessibility guidelines

## 🔧 Utility Classes

### Spacing
```css
.p-sm { padding: 12px; }
.p-md { padding: 16px; }
.p-lg { padding: 24px; }
.p-xl { padding: 32px; }

.m-sm { margin: 12px; }
.m-md { margin: 16px; }
.m-lg { margin: 24px; }
.m-xl { margin: 32px; }
```

### Text
```css
.gradient-text { /* gradient text effect */ }
.text-center { text-align: center; }
.text-bold { font-weight: 700; }
.text-extrabold { font-weight: 800; }
```

### Effects
```css
.glass { /* glass morphism effect */ }
.neomorphic { /* neumorphism effect */ }
.shadow-sm { /* small shadow */ }
.shadow-md { /* medium shadow */ }
.shadow-lg { /* large shadow */ }
```

---

**Version**: 2.0
**Last Updated**: December 1, 2025
**Maintained By**: Design Team
