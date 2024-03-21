# Survey Form - Certification Project

## HTML file
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Survey Form</title>
        <link rel="stylesheet" href="styles.css">
    </head>
    <main>
        <body>
            <div>
                <h1 id="title">Survey Form</h1>
                <p id="description">A simple interview, please answer accordingly</p>
            </div>
            <form id="survey-form">
                <!--Name/Email/Age-->
                <fieldset class="container">
                    <label for="name" id="name-label">Enter your name: <input class="name-email-age-text" id="name" name="name" type="text" placeholder="Your name..." required/> </label>
                    <label for="email" id="email-label">Enter your email: <input class="name-email-age-text" id="email" name="email" type="email" placeholder="Your email..." required/> </label>
                    <label for="number" id="number-label">Enter your age (optional) :  <input class="name-email-age-text" id="number" name="age" type="number" placeholder="Your age..." min="10" max="120" /></label>
                </fieldset>
                <!--Marital Status (Dropdown)-->
                <fieldset>
                    <label for="referrer"> What's your marital status? 
                        <select id="dropdown" name="referrer"> 
                            <option value="">(Select One)</option>
                            <option value="married">Married</option>
                            <option value="widowed">Widowed</option>
                            <option value="separated">Separated</option>
                            <option value="divorced">Divorced</option>
                            <option value="single">Single</option>
                        </select>
                    </label>
                </fieldset>
                <!--Person type (Radio)-->
                <fieldset>
                    <legend>Are you a dog or cat person?</legend>
                    <label class="inline-label"><input id="both" name="person-pet-type" value="both" type="radio" class="inline" checked/>Both!!</label>
                    <label class="inline-label"><input id="dog"  name="person-pet-type" value="dog"  type="radio" class="inline"/>Dog</label>
                    <label class="inline-label"><input id="cat"  name="person-pet-type" value="cat"  type="radio" class="inline"/>Cat</label>
                    <label class="inline-label"><input id="none" name="person-pet-type" value="none" type="radio" class="inline"/>None</label>
                </fieldset>
                <!-- Methods of Transportation(Checkbox)-->
                <fieldset >
                    <legend>Which transportation methods do you prefer?</legend>
                    <label class="inline-label"><input id="transport1" class="inline" name="transport1" value="car" type="checkbox">Car</label>
                    <label class="inline-label"><input id="transport2" class="inline" name="transport2" value="bike" type="checkbox">Bike</label>
                    <label class="inline-label"><input id="transport3" class="inline" name="transport3" value="motorcycle" type="checkbox">Motorcycle</label>
                    <label class="inline-label"><input id="transport4" class="inline" name="transport4" value="bus" type="checkbox">Bus</label>
                    <label class="inline-label"><input id="transport5" class="inline" name="transport5" value="subway" type="checkbox">Subway</label>
                    <label class="inline-label"><input id="transport6" class="inline" name="transport6" value="walking" type="checkbox">Walking</label>
                </fieldset>
                <!--(Textarea)-->
                <fieldset>
                    <label for="bio">Provide a description of yourself:
                        <textarea class="name-email-age-text" id="bio" name="bio" placeholder="Hello, I'm ..."></textarea>
                    </label>

                </fieldset>
                <input id="submit" type="submit" value="Submit"/>
                <footer>
                    <p>Github - <a href="https://github.com/Joviviz">Joviviz</a></p>
                </footer>
            </form>
        </body>
    </main>
</html>
```

## CSS file
```css
body {
    background-color: #1b1b32;
    color: #f5f6f7;
    font-family: Tahoma;
    font-size: 20px;
    
}

h1, p{
    text-align: center;
}

fieldset{
    border: none;
    padding: 2em auto;
}

input,
textarea,
select {
  margin: 5px 0 0 0;
  width: 100%;
  min-height: 2em;
}

form{
    background-color: #282849;
    margin: 0 1em;
    display: block;
    padding: 0.75em 2em 1em;
    border-radius: 25px;
}

.container{
    display: flex;
    flex-direction: column;
    gap: 17px;
    margin-bottom: 30px;
}

.inline-label{
    display: flex;
    align-items: center;
    gap: 10px;
}

.inline{
    width: unset;
    margin-bottom: 4px;
    
}

.name-email-age-text:hover{
    box-shadow: 0 0 10px rgba(0,0,0,.3);
}

label{
    display: block;
}

input, textarea {
    background-color: #131325;
    border: 1px solid #0a0a23;
    color: #ffffff;
}


input[type='submit']{
    margin: 1em auto;
    display: block;
    border-radius: 10px;
    background-color: rgb(107, 188, 115);
}

input[type='submit']:hover{
    background-color: rgb(71, 121, 76);
}

::placeholder{
    color: #ffffff;
    opacity: 50%;
}

a{
    color:rgb(164, 97, 227);
}
```
