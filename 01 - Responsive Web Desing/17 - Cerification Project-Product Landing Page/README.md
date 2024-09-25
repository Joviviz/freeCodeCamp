# 

## <ins>Objective :<ins>
### 
### 

## HTML File
```html
<!DOCTYPE html>
<html lang="en">

  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="styles.css" />
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />
    
    <title>Product Landing Page</title>
  </head>

  <body>
    <header id="header" >
      <div id="div-img">
        <img 
        id="header-img" 
        src="https://static.vecteezy.com/system/resources/previews/006/622/216/original/guitar-outline-icon-isolated-on-a-white-background-acoustic-guitar-symbol-for-web-and-mobile-app-illustrations-free-vector.jpg" 
        >
        <h1> Original Guitars </h1>
      </div>
      
        
        <nav id="nav-bar" >
          <ul>
            <li><a class="nav-link" href="#Pricing" >Pricing</a></li>
            <li><a class="nav-link" href="#How-it-works" >How It Works</a></li>
            <li><a class="nav-link" href="#Features" >Features</a></li>
          </ul>
        </nav>
    </header>
    <main>
      <div id="email-div">
        <h1>Tune in to your habilities</h1>
        <form id="form" action="https://www.freecodecamp.com/email-submit">
          <input 
            id="email" 
            name="email"
            placeholder="Email goes here!"
            type="email"
          >
          <input
            id="submit"
            type="submit"
            value="Get Started"
            class="button"
          >
        </form>
      </div>
      
      <section id="Features">

        <div class="grid">
          <div class="icon">
            <span class="material-symbols-outlined feature-symbol icon-large">local_fire_department</span>
          </div>
          <div class="desc">
            <h2 class="desc-text">Quality Assurance & Lifetime Warranty</h2>
            <p class="desc-text">
              Our primary selling point is the
              strong emphasis on high-quality craftsmanship 
              and durability. We proudly offer an extended 
              warranty on our guitars, demonstrating our commitment to 
              the longevity and exceptional quality of our instruments.
            </p>

          </div>
        </div>

        <div class="grid">
          <div class="icon">
            <span class="material-symbols-outlined icon-large">brush</span>
          </div>
          <div class="desc">
            <h2 class="desc-text">Customization</h2>
            <p class="desc-text">
              Now, more than ever, you can fully customize your guitar to 
              fit your unique style and preferences. This option appeals 
              to both seasoned players and beginners looking for a truly 
              personal instrument.
            </p>

          </div>
        </div>

        <div class="grid">
          <div class="icon">
            <span class="material-symbols-outlined icon-large">music_note</span>
          </div>
          <div class="desc">
            <h2 class="desc-text">Play Before You Pay</h2>
            <p class="desc-text">
              Online buyers enjoy a 30-day trial period to test the guitar. 
              If it's not the perfect fit, return it with free shipping—no 
              questions asked!
            </p>

          </div>
        </div>
        <div class="grid">
          <div class="icon">
            <span class="material-symbols-outlined icon-large">nature</span>
          </div>
          <div class="desc">
            <h2 class="desc-text">Eco-Friendly Models</h2>
            <p class="desc-text">
              We cater to environmentally-conscious customers by offering 
              eco-friendly guitars made from sustainable or reclaimed woods, 
              packaged in recyclable materials.
            </p>

          </div>
        </div>

      </section>

      <section id="How-it-works">
        <iframe id="video" class="video" src="https://www.youtube.com/embed/Y-33v7bJLIc" 
          frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
          allowfullscreen>
        </iframe>
      </section>
      
      <section id="Pricing">
        <div class="price-grid">
          <h3 class="product-title" >Dreadnought Guitar</h3>
          <h2>$12.000</h2>
          <div class="product-desc">
            <p>Lorem ipsum.</p>
            <p>ipsum.</p> 
            <p>Lorem ipsum dolor.</p>
            <p>Lorem ipsum.</p>
          </div>

          <button class="btn-product" type="button">Select</button>
        </div>
        <div class="price-grid">
          <h3 class="product-title" >Orchestra Guitar</h3>
          <h2>$2.900</h2>
          <div class="product-desc">
            <p>Lorem ipsum.</p>
            <p>ipsum.</p> 
            <p>Lorem ipsum dolor.</p>
            <p>Lorem ipsum.</p>
          </div>

          <button class="btn-product" type="button">Select</button>
        </div>
        <div class="price-grid">
          <h3 class="product-title" >Parlor Guitar</h3>
          <h2>$950</h2>
          <div class="product-desc">
            <p>Lorem ipsum.</p>
            <p>ipsum.</p> 
            <p>Lorem ipsum dolor.</p>
            <p>Lorem ipsum.</p>
          </div>

          <button class="btn-product" type="button">Select</button>
        </div>

      </section>

      <p id="github-link" style="text-align: center; "><a id="github-link" style="text-decoration: none;" href='https://github.com/Joviviz' target="_blank">Joviviz</a></p>
      
    </main>
  </body>

</html>
```

## CSS File
```css
:root{
  --vibrant-yellow: rgb(255, 208, 0);
  --vibrant-yellow-hover: rgb(255, 231, 126);
}

body{
  margin: 0;
  padding: 0;
}

#header{
  width: 100%;
  height: 75px;
  position: fixed;
  top: 0;
  border-bottom: solid black;
  background-color: white;
  z-index: 1000;
}

#div-img{
  display: flex;
  float: left;
  height: 75px;
  width: 50%;
  background-color: white;
  z-index: 100;
}

#div-img h1{
  display: flex;
  margin: auto 0;
  align-items: center;
}

#header-img{
  width: auto;
  height: 75px;
  float: left;
  z-index: 100;
}

#nav-bar{
  height: 75px;
  width: 50%;
  float: right;
  z-index: 9999;
}

#nav-bar ul{
  overflow: hidden;
  list-style-type: none;
  height: 75px;
  margin: 0;
  padding: 0;
  align-items: center;
}

#nav-bar li{
  float: right;
}

#nav-bar a{
  display: block;
  text-decoration: none;
  color: black;
  padding: 29px 30px;
  border-left: solid 2px black;
  text-align: center;
}

#nav-bar a:hover{
  background-color: grey;
}

#email-div{
  width: 50%;
  text-align: center;
  justify-content: center;
  margin: 0 auto;
  margin-bottom: 30px;
}

#email{
  max-width: 275px;
  width: 100%;
}

.button{  
  display: block;
  margin: 0 auto;
  justify-content: center;
  text-transform: uppercase;
  background: black;
  color: white;
  padding: 10px;
  margin-top: 15px;
  font-weight: 1000;
}

.button:hover{
  background: grey;
  cursor: pointer;
}

#Features{
  display: flex;
  text-align: center;
  flex-direction: column;
  visibility: visible !important;
}

.grid{
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.icon{
    display: flex;
    align-items: center;
    justify-content: center;
    height: 125px;
    width: 20vw;
}

.icon-large {
  transform: scale(2);
  z-index: 1;
  color: var(--vibrant-yellow);
}

.desc{
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 125px;
  width: 80vw;
  margin-right: 30px;
}

.desc-text{
  margin: 0;
  text-align: left;
}

main {
  margin: 0 auto;
  padding-top: 100px;
  font-family: 'Lato', sans-serif;
}


#How-it-works{
  margin-top: 30px;
  margin-bottom: 30px;
  display: flex;
  justify-content: center;
}

.video{
  width: 700px;
  height: 315px;
}

#Pricing{
  
  display: flex;
  justify-content: center;
  flex-direction: row;
  margin-bottom: 100px; 
}

.price-grid{
  height: 350px;
  width: 270px;
  border: solid black 3px;
  margin: 10px;
  text-align: center;
}

.product-title{
  margin: 0;
  padding: 25px;
  background-color: var(--vibrant-yellow) ;
}

.product-desc{
  margin-bottom: 30px;
}

.product-desc>p{
  margin: 10px;
}

.btn-product{
  display: block;
  margin: 0 auto;
  justify-content: center;
  text-transform: uppercase;
  background: var(--vibrant-yellow);
  padding: 10px;
  font-weight: 600;
  width: 50%;
  font-size: 20px;
}

.btn-product:hover{
  background: var(--vibrant-yellow-hover);
  cursor: pointer;
}

@media (max-width: 450px){
  .nav-link{
    font-size: 12px;
  }
  .desc{
    height: 170px;
  }
}

@media (max-width: 650px){

  .icon{
    display: none;
  }
  
  .desc{
    margin-left: 5%;
    font-size: 14px;
  }
}

@media (max-width: 775px){
  #header{
    height: 150px;
  }

  #div-img{
    width: 100%;
    justify-content: center;
    float: none;
  }

  #div-img h1{
    justify-content: center;
  }

  #nav-bar{
    width: 100%;
  }

  #nav-bar ul{
    justify-content: center;
    float: none;
  }

  #nav-bar li{
    width: 33.333%;
    border-top: solid 2px black;
  }

  #nav-bar>ul>li:last-child>a{
    border-left: 0;
  }

  main{
    padding-top: 180px ;
  }

  #Pricing{
    flex-direction: column;
    align-items: center;
  }


}




```