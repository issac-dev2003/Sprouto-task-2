# Sprouto-task-2

Task 2: Build a basic Webpage Using HTML, CSS and JS for animations
The page should be composed of the following:
* Nav Bar
* Animated Slider/ Carousel/ Hero section with 5 Images
* Products Cards section (12 Products)
* Animated Reviews section
* Footer
---------------------------------------------------------------------------------


# 📄 Project Documentation: Animated Webpage with Slider, Products, and Reviews
✅ Overview
This project is a basic responsive webpage designed using HTML, CSS, and JavaScript. It includes key UI components commonly found in modern websites:

- Navigation bar
- Animated hero slider
- Products grid section
- Auto-scrolling reviews section
- Footer


## 🛠 Technologies Used

- **HTML** – Page structure
- **CSS** – Styling and layout
- **JavaScript** – Dynamic content generation (product cards)

## 📁 File Structure
index.html         ← Main file with all HTML, CSS, and JS

## 🧱 Component Structure

### 🔝 Navigation Bar

- Uses Flexbox for alignment
- Links to different sections using anchor tags
- Dark background with white text for contrast

```html
<nav>
  <div class="logo">My Store</div>
  <div>
    <a href="#">Home</a>
    <a href="#products">Products</a>
    <a href="#reviews">Reviews</a>
    <a href="#contact">Contact</a>
  </div>
</nav>
```
### 🎞️ Hero Image Slider

- Horizontally scrollable image slider using scroll-snap-type
- Smooth scrolling behavior with clickable dot navigation
- 5 Unsplash images used for demo

  ```
  <section class="container">
  <div class="slider-wrapper">
    <div class="slider">
      <img id="slide-1" src="..." />
      ...
    </div>
    <div class="slider-nav">
      <a href="#slide-1"></a>
      ...
    </div>
  </div>
  </section>
  ```
### 🛍 Product Cards

- Grid layout using CSS Grid (repeat(auto-fit, minmax(...)))
- Dynamically generated using JavaScript
- Hover animation for interactive effect

    ```JS
  for(let i = 1; i <= 12; i++) {
  document.write(`
    <div class="product-card">
      <img src="https://picsum.photos/seed/product${i}/200/150" alt="Product ${i}" />
      <h3>Product ${i}</h3>
      <p>$${(i * 10).toFixed(2)}</p>
    </div>
  `);
  }

  ```


###💬 Reviews Section

- Auto-scrolling horizontal animation using CSS @keyframes
- Displays multiple review cards that scroll endlessly

    ```
  <section id="reviews" class="reviews">
  <div class="review-container">
    <div class="review">"Great product! Highly recommend."</div>
    ...
  </div>
  </section>

  ```

### 🔚 Footer

- Simple footer with white text on a dark background

```
 <footer>
 &copy; 2025 My Store. All rights reserved.
 </footer>

```

### 🎨 Styling Notes
Layout structured using Flexbox and Grid

- Smooth scroll effects in slider
- Hover effects for interactivity
- Hidden scrollbars in slider using ::-webkit-scrollbar and similar properties

###📷 Image Sources
- Slider Images: Unsplash
- Product Images: Picsum Photos
