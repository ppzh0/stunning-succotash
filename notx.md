# code block backup

## HTML
```html
<article class="card">
    <h2 class="cardH">Title</h2>
    <div class="content-wrapper">
        <img src="assets/img/*" alt="" class="cardP">
        <ul class="cardI">
            <li>Artist</li>
            <li>Genre</li>
            <li>Type</li>
        </ul>
    </div>
    <div class="btn-wrapper">
        <a href="" class="btn youtube">YouTube</a>
        <a href="" class="btn spotify">Spotify</a>
    </div>
</article>
```
## CSS
```css
.card {
    border-radius: var(--px);
    margin-top: 3rem;
    transition: all .3s ease-out;
}

.card:hover {
    box-shadow: -4px 7px 20px 0 rgb(0 0 0 / 30%), 2px 0 20px 0 rgb(0 0 0 / 30%);
}

.cardH {
    padding: 1rem .3rem 0;
    /* text stuff */
    text-align: center;
}

.content-wrapper {
    /* display stuff */
    display: grid;
    /* makes the image and info aligned center */
    grid-template-columns: repeat(2, auto);
    align-items: center;
    justify-items: center;
    margin: 0 .6rem;
    word-break: break-all;
    text-align: end;
}

.content-wrapper ul {
    list-style: none;
    padding-inline-start: 0;
}

.cardP {
    /* default display */
    width: calc(85px + 3vw);
    border-radius: var(--px);
}

/* buttons */
.btn-wrapper {
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
    border-bottom-right-radius: var(--px);
}

.spotify:hover {
    background-color: #191414;
    color: #1DB954;
}

.youtube {
    font-family: "YouTubeSans";
    border-bottom-left-radius: var(--px);
}

.youtube:hover {
    background-color: #FF0000;
    color: #282828;
}
```