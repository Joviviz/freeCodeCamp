# CSS Colored Markers
## <ins>Objective :<ins>

### This Project aims to build a set of colored markers.
### It uses different ways to set color values (RGBA, HEX, HSLA), pairing colors with each other and using functions such as "color-gradient" and "box-shadow" to create light based reflections and shadows.

# HTML file
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Colored Markers</title>
    <link rel="stylesheet" href="styles.css">
  </head>
  <body>
    <main>
      <h1>CSS Color Markers</h1>
      <div class="container">
        <div class="marker red">
          <div class="cap"></div>
          <div class="sleeve"></div>
        </div>
        <div class="marker green">
          <div class="cap"></div>
          <div class="sleeve"></div>
        </div>
        <div class="marker blue">
          <div class="cap"></div>
          <div class="sleeve"></div>
        </div>
      </div>
    </main>
    <footer>
      <br>
      <p>-</p>
      <p>
        Visit my github : <a href="https://github.com/Joviviz" target="_blank">Joviviz</a>
      </p>
    </footer>
  </body>
</html>
```
# CSS file

```css
h1 {
    text-align: center;
  }
  
  .container {
    background-color: rgb(255, 255, 255);
    padding: 10px 0;
  }
  
  .marker {
    width: 200px;
    height: 25px;
    margin: 10px auto;
  }
  
  .cap {
    width: 60px;
    height: 25px;
  }
  
  .sleeve {
    width: 110px;
    height: 25px;
    background-color: rgba(255, 255, 255, 0.5);
    border-left: 10px double rgba(0, 0, 0, 0.75);
  }
  
  .cap, .sleeve {
    display: inline-block;
  }
  
  .red {
    background: linear-gradient(rgb(122, 74, 14), rgb(245, 62, 113), rgb(162, 27, 27));
    box-shadow: 0 0 20px 0 rgba(83, 14, 14, 0.8);
  }
  
  .green {
    background: linear-gradient(#55680D, #71F53E, #116C31);
    box-shadow: 0 0 20px 0 #3B7E20CC;
  }
  
  .blue {
    background: linear-gradient(hsl(186, 76%, 16%), hsl(223, 90%, 60%), hsl(240, 56%, 42%));
    box-shadow: 0 0 20px 0 hsla(223, 59%, 31%, 0.8);
  }

  footer{
    font-size: 16px;
    text-align: center;
  }
```
