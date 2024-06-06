# Piano! - Responsive Web Desing

## <ins>Objective :<ins>
### Responsive Design tells your webpage how it should look on different-sized screens.

### Build a piano using media queries and pseudo selectors.


## HTML File
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <title>Piano</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="./styles.css">
  </head>
  <body>
    <div id="piano">
      <img class="logo" src="https://cdn.freecodecamp.org/platform/universal/fcc_primary.svg" alt="freeCodeCamp Logo" />
      <div class="assinatura">
        <p class="signature"><a href='https://github.com/Joviviz' target="_blank">Joviviz</a></p>
      </div>
      <div class="keys">
        <div class="key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
        <div class="key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>

        <div class="key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
        <div class="key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>

        <div class="key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
        <div class="key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
        <div class="key black--key"></div>
      </div>
    </div>
  </body>
</html>
```

## CSS File
```css
html {
    box-sizing: border-box;
  }
  
  *, *::before, *::after {
    box-sizing: inherit;
  }
  
  #piano {
    background-color: #00471b;
    width: 992px;
    height: 290px;
    margin: 80px auto;
    padding: 90px 20px 0 20px;
    position: relative;
    border-radius: 10px;
  }
  
  .keys {
    background-color: #040404;
    width: 949px;
    height: 180px;
    padding-left: 2px;
    overflow: hidden;
  }
  
  .key {
    background-color: #ffffff;
    position: relative;
    width: 41px;
    height: 175px;
    margin: 2px;
    float: left;
    border-radius: 0 0 3px 3px;
  }
  
  .key.black--key::after {
    background-color: #1d1e22;
    content: "";
    position: absolute;
    left: -18px;
    width: 32px;
    height: 100px;
    border-radius: 0 0 3px 3px;
  }
  
  .logo {
    width: 200px;
    position: absolute;
    top: 23px;
  }

  .signature{
    position: absolute;
    top: 23px;
    right: 20px;
    margin: 0 auto;
  }
  
  @media (max-width: 768px) {
    #piano {
      width: 358px;
    }
  
    .keys {
      width: 318px;
    }
  
    .logo {
      width: 150px;
    }

  }
  
  @media (max-width: 1199px) and (min-width: 769px) {
    #piano{
      width: 675px;
    }
    .keys{
      width: 633px;
    }
  }



  a:link {color:#ffffff;}
  a:visited {color:#ffffff;}
  a:hover {color:#9fd7bf;}
```