# code block backup

## HTML
```html
<article class="card">
    <h2 class="header">The Best For You</h2>
    <div class="wraps">
        <img src="assets/img/the-best-for-you.jpg" alt="" class="img">
        <div class="cardI">
            <fieldset>
                <legend>Artist<legend>
                Hikaru Station, Redza
            </fieldset>
            <fieldset>
                <legend>Album</legend>
                The Best For You
            </fieldset>
        </div>
    </div>
    <div class="wrapsBTN">
        <a href="" class="btn youtube">YouTube</a>
        <a href="" class="btn spotify">Spotify</a>
    </div>
</article>
```
## CSS
```css
.card {
    border-radius: var(--dP);
    margin-top: 3rem;
    transition: all .3s ease-out;
}

.card:hover {
    box-shadow: -4px 7px 20px 0 rgb(0 0 0 / 30%), 2px 0 20px 0 rgb(0 0 0 / 30%);
}

.header {
    padding: 1rem .3rem 0;
    /* text stuff */
    text-align: center;
}

.cardI {
    width: 90%;
    text-align: right;
    padding: 0.4rem;
}

.wraps {
    /* display stuff */
    display: grid;
    /* makes the image and info aligned center */
    grid-template-columns: repeat(2, auto);
    align-items: center;
    justify-items: center;
}

.wraps ul {
    list-style: none;
    padding-inline-start: 0;
}

.img {
    /* default display */
    width: calc(100px + 3vw);
    border-radius: calc(var(--dP) / 2);
    padding-left: .8rem;
}

/* buttons */
.wrapsBTN {
    /* display stuff */
    /* makes buttons aligned center */
    display: grid;
    grid-template-columns: repeat(2, auto);
    /* put a bit of space between content wrapper */
    margin-top: 1rem;
}

.btn {
    padding: .8rem 1rem;
    /* text stuff */
    text-align: center;
    text-decoration: none;
    color: #000;
    font-weight: bold;
    /* animation stuff */
    transition: all .3s ease;
}

/* button styles */
.spotify {
    font-family: Gotham;
    border-bottom-right-radius: var(--dP);
}

.spotify:hover {
    background-color: #191414;
    color: #1DB954;
}

.youtube {
    font-family: "YouTubeSans";
    font-weight: bolder;
    border-bottom-left-radius: var(--dP);
}

.youtube:hover {
    background-color: #FF0000;
    color: #282828;
}
```