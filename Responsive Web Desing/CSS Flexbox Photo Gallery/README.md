# CSS Flexbox Photo Gallery
## <ins>Objective :<ins>
### UIse Flexbox to build a responsive photo gallery webpage.

## HTML file
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Photo Gallery</title>
    <link rel="stylesheet" href="./styles.css">
  </head>
  <body>
    <header class="header">
      <h1>css flexbox photo gallery</h1>
    </header>
    <div class="gallery">
      <img alt='cat-sleep' src="https://cdn.freecodecamp.org/curriculum/css-photo-gallery/1.jpg">
      <img alt='cat-strech' src="https://cdn.freecodecamp.org/curriculum/css-photo-gallery/2.jpg">
      <img alt='cat-look' src="https://cdn.freecodecamp.org/curriculum/css-photo-gallery/3.jpg">
      <img alt='cat-sleep2' src="https://cdn.freecodecamp.org/curriculum/css-photo-gallery/4.jpg">
      <img alt='cat-stare' src="https://cdn.freecodecamp.org/curriculum/css-photo-gallery/5.jpg">
      <img alt='cat-cuddles' src="https://cdn.freecodecamp.org/curriculum/css-photo-gallery/6.jpg">
      <img alt='cat-blanket' src="https://cdn.freecodecamp.org/curriculum/css-photo-gallery/7.jpg">
      <img alt='cat-stare2' src="https://cdn.freecodecamp.org/curriculum/css-photo-gallery/8.jpg">
      <img alt='cat-cuddles2' src="https://cdn.freecodecamp.org/curriculum/css-photo-gallery/9.jpg">
```

## CSS File
```css
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: sans-serif;
  background: #f5f6f7;
}

.header {
  text-align: center;
  text-transform: uppercase;
  padding: 32px;
  background-color: #0a0a23;
  color: #fff;
  border-bottom: 4px solid #fdb347;
}

.gallery {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  gap: 16px;
  max-width: 1400px;
  margin: 0 auto;
  padding: 20px 10px;
}

.gallery img {
  width: 100%;
  max-width: 350px;
  height: 300px;
  object-fit: cover;
  border-radius: 10px;
}

.gallery::after {
  content: "";
  width: 350px;
}

```
