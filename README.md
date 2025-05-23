# Claude Ribbons

GitHub-style corner ribbons with "Built with Claude" text. Perfect for showcasing projects built using Claude AI. Inspired by [GitHub Ribbons](https://github.blog/news-insights/the-library/github-ribbons/).

Demo: https://claude-ribbons.netlify.app/

## Features

- Clean, professional ribbon design
- Multiple color variations
- Hover effects with smooth transitions  
- Responsive design
- Easy to customize
- Works on any website

## Basic Usage

Add the ribbon CSS to your stylesheet and include the HTML element where you want the ribbon to appear.

### Top Right Ribbon (Default Blue)

```html
<div class="container">
  <a href="#" class="ribbon-top-right">Built with Claude</a>
  <!-- Your content here -->
</div>
```

```css
.container {
  position: relative;
  /* your container styles */
}

.ribbon-top-right {
  position: absolute;
  top: 25px;
  right: -35px;
  background: #007acc;
  color: white;
  padding: 10px 50px;
  text-decoration: none;
  font-weight: bold;
  font-size: 14px;
  transform: rotate(45deg);
  box-shadow: 0 2px 5px rgba(0,0,0,0.3);
  transition: background-color 0.3s;
  width: 150px;
  text-align: center;
}

.ribbon-top-right:hover {
  background: #005999;
}
```

### Top Left Ribbon (Green)

```html
<div class="container">
  <a href="#" class="ribbon-top-left">Built with Claude</a>
  <!-- Your content here -->
</div>
```

```css
.ribbon-top-left {
  position: absolute;
  top: 60px;
  left: -60px;
  background: #28a745;
  color: white;
  padding: 10px 50px;
  text-decoration: none;
  font-weight: bold;
  font-size: 14px;
  transform: rotate(-45deg);
  box-shadow: 0 2px 5px rgba(0,0,0,0.3);
  transition: background-color 0.3s;
  width: 150px;
  text-align: center;
}

.ribbon-top-left:hover {
  background: #1e7e34;
}
```

## Color Variations

You can add these additional CSS classes for different color schemes:

### Red Ribbon

```html
<a href="#" class="ribbon-top-right ribbon-red">Built with Claude</a>
```

```css
.ribbon-red {
  background: #dc3545 !important;
}

.ribbon-red:hover {
  background: #c82333 !important;
}
```

### Purple Ribbon

```html
<a href="#" class="ribbon-top-right ribbon-purple">Built with Claude</a>
```

```css
.ribbon-purple {
  background: #6f42c1 !important;
}

.ribbon-purple:hover {
  background: #5a32a3 !important;
}
```

### Dark Ribbon

```html
<a href="#" class="ribbon-top-left ribbon-dark">Built with Claude</a>
```

```css
.ribbon-dark {
  background: #343a40 !important;
}

.ribbon-dark:hover {
  background: #23272b !important;
}
```

## Complete CSS

Here's the complete CSS for all ribbon variations:

```css
/* Base ribbon styles */
.ribbon-top-right {
  position: absolute;
  top: 25px;
  right: -35px;
  background: #007acc;
  color: white;
  padding: 10px 50px;
  text-decoration: none;
  font-weight: bold;
  font-size: 14px;
  transform: rotate(45deg);
  box-shadow: 0 2px 5px rgba(0,0,0,0.3);
  transition: background-color 0.3s;
  width: 150px;
  text-align: center;
}

.ribbon-top-right:hover {
  background: #005999;
}

.ribbon-top-left {
  position: absolute;
  top: 60px;
  left: -60px;
  background: #28a745;
  color: white;
  padding: 10px 50px;
  text-decoration: none;
  font-weight: bold;
  font-size: 14px;
  transform: rotate(-45deg);
  box-shadow: 0 2px 5px rgba(0,0,0,0.3);
  transition: background-color 0.3s;
  width: 150px;
  text-align: center;
}

.ribbon-top-left:hover {
  background: #1e7e34;
}

/* Color variations */
.ribbon-red {
  background: #dc3545 !important;
}

.ribbon-red:hover {
  background: #c82333 !important;
}

.ribbon-purple {
  background: #6f42c1 !important;
}

.ribbon-purple:hover {
  background: #5a32a3 !important;
}

.ribbon-dark {
  background: #343a40 !important;
}

.ribbon-dark:hover {
  background: #23272b !important;
}
```

## Important Notes

- Make sure your ribbon's parent container has `position: relative`
- The ribbon needs `overflow: hidden` on the parent container to clip properly
- Ribbons work best on containers with adequate padding/margin at the corners
- Text length affects the ribbon appearance - keep it concise

## Customization

### Change the Text

Simply replace "Built with Claude" with your desired text:

```html
<a href="#" class="ribbon-top-right">Your Text Here</a>
```

### Custom Colors

Create your own color variation:

```css
.ribbon-custom {
  background: #your-color !important;
}

.ribbon-custom:hover {
  background: #your-hover-color !important;
}
```

### Adjust Size

Modify the `width`, `padding`, and `font-size` properties:

```css
.ribbon-large {
  width: 200px;
  padding: 15px 60px;
  font-size: 16px;
}
```

## Browser Support

- All modern browsers
- IE11+ (with some CSS3 limitations)
- Mobile responsive

## License

Free to use in any project. No attribution required.
