# J.J. Thomson Tribute Website

## <ins>Objective :<ins>
### Build a Tribute Page, Build an app that is functionally similar to https://tribute-page.freecodecamp.rocks. Do not copy this demo project.

User Stories:

- Your tribute page should have a main element with a corresponding id of main, which contains all other elements
- You should see an element with an id of title, which contains a string (i.e. text), that describes the subject of the tribute page (e.g. "Dr. Norman Borlaug")
- You should see either a figure or a div element with an id of img-div
- Within the #img-div element, you should see an img element with a corresponding id="image"
- Within the #img-div element, you should see an element with a corresponding id="img-caption" that contains textual content describing the image shown in #img-div
- You should see an element with a corresponding id="tribute-info", which contains textual content describing the subject of the tribute page
- You should see an a element with a corresponding id="tribute-link", which links to an outside site, that contains additional information about the subject of the tribute page. HINT: You must give your element an attribute of target and set it to _blank in order for your link to open in a new tab
- Your #image should use max-width and height properties to resize responsively, relative to the width of its parent element, without exceeding its original size
- Your img element should be centered within its parent element

Fulfill the user stories and pass all the tests below to complete this project. Give it your own personal style. Happy Coding!

- Note: Be sure to add <link rel="stylesheet" href="styles.css"> in your HTML to link your stylesheet and apply your CSS

## HTML File
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8"/>
        <meta name="viewport" content="width=device-width, initial-scale=1"/>
        <title>Tribute Page</title>
        <link rel="stylesheet" href="styles.css"/>
    </head>
    <body>
        <main id="main">
            <h1 id="title" class="title">Joseph John Thomson</h1>
            <p id="title" class="title" >The man that revolutionized atomic studies</p>
            <div id="img-div">
                <img id="image" src="https://cdn.discordapp.com/attachments/1224065809576366200/1224076126645784737/800px-Sir_J.J._Thomson_LCCN2014715407_1.jpg?ex=661c2cba&is=6609b7ba&hm=6993e96e8d4dfa3378b04443b70e86122bdbcc5b9dc657bfbff2717966b1421d&" alt="tributed-person-img"  >
                <figcaption id="img-caption">A vintage portrait photo circa 1900s of our beloved British physicist Sir Joseph John "J. J." Thomson - winner of the Nobel Prize in Physics</figcaption>
            </div>
            <nav>
                <ul>
                    <li><p><strong>1856</strong> - Born December 18 at Cheetham Hill, near Manchester</p></li>
                    <li><p><strong>1876</strong> - Joined the Trinity College at Cambridge</p></li>
                    <li><p><strong>1880</strong> - Obtained his Bachelor of Arts degree in mathematics</p></li>
                    <li><p><strong>1884</strong> - Elected as a fellow of the Royal Society, a national scientific society and appointed for a chair of physics at the Cavendish Laboratory</p></li>
                    <li><p><strong>1890</strong> - Married his wife Rose Elizabeth Paget</p></li>
                    <li><p><strong>1897</strong> - Discovered the existance of the electron</p></li>
                    <li><p><strong>1904</strong> - Suggests a discontinuous theory of light, foreshadowing Albert Einstein’s later theory of photons</p></li>
                    <li><p><strong>1906</strong> - Received the Nobel Prize for Physics for his researches into the electrical conductivity of gases </p></li>
                    <li><p><strong>1908</strong> - Was made a knight</p></li>
                    <li><p><strong>1909</strong> - Made president of the British Association for the Advancement of Science</p></li>
                    <li><p><strong>1910</strong> - Motivated Ernest Rutherford to research that lead to the modern understanding of the internal structure of the atom, AKA the Rutherford atomic model</p></li>
                    <li><p><strong>1912</strong> - Received the Order of Merit, a reward to those who particularly distinguished themselves in science, art, literature, or the promotion of culture</p></li>
                    <li><p><strong>1918</strong> - Made master of Trinity College</p></li>
                    <li><p><strong>1940</strong> - Died August 30 at Cambridge, Cambridgeshire</p></li>
                </ul>
            </nav>
            <div id="info-div">
                <p id="tribute-info">"As we conquer peak after peak we see in front of us regions full of interest and beauty, but we do not see our goal, we do not see the horizon; in the distance tower still higher peaks, which will yield to those who ascend them still wider prospects, and deepen the feeling, the truth of which is emphasized by every advance in science, that ' Great are the Works of the Lord ' ".</p>
                <p id="signature">- - <strong>J.J. Thomson</strong> </p>
            </div>
            <p id="tribute-paralink">To read more about J.J. Thomson's biography click <a href="https://www.britannica.com/biography/J-J-Thomson" id="tribute-link" target="_blank" >here!</a>
            <p id="github-link"> - <br/></p><a id="github-link" href='https://github.com/Joviviz' target="_blank">Joviviz</a></p>
        </main>
    </body>
</html>
```

## CSS File
```css

body{
    background-image: url(https://cdn.discordapp.com/attachments/1224065809576366200/1224065912349397154/image-from-rawpixel-id-5924106-jpeg.jpg?ex=661c2337&is=6609ae37&hm=be43fa8e87301efa1dfa9ad6fd48544a711449a1f170a8d152bc94c182b28156&);
    font-family: Arial, Helvetica, sans-serif;
}

main{
    background: #131323;
    background: linear-gradient(180deg, hsla(240, 30%, 11%, 1) 0%, rgb(31, 29, 69) 100%);
    color: #f5f6f7;
    margin: 0;
    width: 95%;
    margin-left: auto;
    margin-right: auto;

}

#title{
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 auto;
}

h1.title{
    padding: 0.75em;
}

p.title {
    color: rgb(207, 217, 225);
    padding-bottom: 1em;
}

#img-div{
    display: block;
    justify-content: center;
    background-color:rgb(47, 47, 74);
    width: 98%;
    padding-top: 0;
    padding-bottom: 2em;
    margin: 0 auto;
    border-radius: 1em;
}

#image{
    display: block;
    max-width: 100%;
    height: auto;
    margin: 0 auto;
    padding-top: 0.2em;

}

#img-caption{
    display: flex;
    justify-content: center;
    font-family:'Times New Roman', Times, serif;
    color: rgb(206, 219, 231);
    padding-top: 1.5em;
    margin: 0 5%;
}

ul{
    display: block;
    justify-content: center;
    width: 55%;
    padding-top: 2em;
    padding-bottom: 2em;
    margin: 0 auto;
}

#info-div{
    display: block;
    justify-content: center;
    width: 95%;
    padding-top: 2em;
    padding-bottom: 2em;
    margin: 0 auto;
    background-color:rgb(47, 47, 74);
    border-radius: 1.5em;
    
}

#tribute-info{
    display: block;
    justify-content: center;
    font-style: italic;
    width: 85%;
    margin: 0 auto;
}

#signature{
    display: block;
    justify-content: center;
    margin: 0 auto;
    padding-top: 1em;
    width: 84%;
}

#tribute-paralink{
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 auto;
    padding-top: 1.5em;
    padding-bottom: 1.5em;
}

#github-link {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 auto;
    padding-bottom: 1.5em;
}

a {padding-left: 0.25em;}
a:link {color:#ffffff;}
a:visited {color:#b9b7dc;}
a:hover {color:#cb8dd9;}
```
