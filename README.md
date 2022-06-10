<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

<style>
    

    
    div.conteiner-carousel {
    display: grid;
    grid-template-rows: 270px 30px;
    grid-template-columns: 1fr 30px 30px 30px 30px 30px 1fr;
    align-items: end;
    justify-items: center;
    
    padding: 20px 0px;
    }

    div#carousel {
    grid-row: 1;
    grid-column: 1 / 8;
    width: 90vw;
    height: 270px;

    padding: 0px 20px;

    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
    transform-style: preserve-3d;
    perspective: 300px;
    }

    div.carousel-item {
    position: absolute;
    width: 400px;
    height: 270px;

    padding: 10px;

    color: rgba(0, 0, 0, 0);
    background-color: rgb(30, 34, 43);
    box-shadow: 10px 0px 18px -8px rgba(31, 20, 20, 0.4),-10px 0px 18px -8px rgba(0,0,0,0.4);

    transition: all 0.4s ease-out;

    --r: calc(var(--position) - var(--offset));
    --abs: max(calc(var(--r) * -1), var(--r));
    
    transform: rotateY(calc(-2deg * var(--r)))
        translateX(calc(-40px * var(--r)));
    z-index: calc((var(--position) - var(--abs)));
    }

    div.carousel-item:hover {
    color: whitesmoke;
    }

    div.carousel-item:nth-of-type(1) {
    --offset: 1;
    }
    div.carousel-item:nth-of-type(2) {
    --offset: 2;
    }
    div.carousel-item:nth-of-type(3) {
    --offset: 3;
    }
    div.carousel-item:nth-of-type(4) {
    --offset: 4;
    }
    div.carousel-item:nth-of-type(5) {
    --offset: 5;
    }


    input:nth-of-type(1) {
    grid-column: 2;
    grid-row: 2;
    }
    input:nth-of-type(1):checked ~ div#carousel {
    --position: 1;
    }
    input:nth-of-type(1):checked ~ div#carousel > div.carousel-item:nth-of-type(1) {
    color: whitesmoke;
    }

    input:nth-of-type(2) {
    grid-column: 3;
    grid-row: 2;
    }
    input:nth-of-type(2):checked ~ div#carousel {
    --position: 2;
    }
    input:nth-of-type(2):checked ~ div#carousel > div.carousel-item:nth-of-type(2) {
    color: whitesmoke;
    }

    input:nth-of-type(3) {
    grid-column: 4;
    grid-row: 2;
    }
    input:nth-of-type(3):checked ~ div#carousel {
    --position: 3;
    }
    input:nth-of-type(3):checked ~ div#carousel > div.carousel-item:nth-of-type(3) {
    color: whitesmoke;
    }

    input:nth-of-type(4) {
    grid-column: 5;
    grid-row: 2;
    }
    input:nth-of-type(4):checked ~ div#carousel {
    --position: 4;
    }
    input:nth-of-type(4):checked ~ div#carousel > div.carousel-item:nth-of-type(4) {
    color: whitesmoke;
    }

    input:nth-of-type(5) {
    grid-column: 6;
    grid-row: 2;
    }
    input:nth-of-type(5):checked ~ div#carousel {
    --position: 5;
    }
    input:nth-of-type(5):checked ~ div#carousel > div.carousel-item:nth-of-type(5) {
    color: whitesmoke;
    }

    input[type="radio"] {
    -webkit-appearance: none;
    appearance: none;
    background-color: rgb(30, 34, 43);

    font: inherit;
    width: 1.15em;
    height: 1.15em;
    border: 0.15em solid rgba(15, 18, 22, 0.5);
    border-radius: 50%;

    display: grid;
    place-content: center;
    }

    input[type="radio"]:hover {
    transition: 120ms ease-out;
    outline: max(2px, 0.15em) solid rgb(15, 18, 22);
    outline-offset: max(2px, 0.15em);
    }

    input[type="radio"]::before {
    content: "";
    width: 0.65em;
    height: 0.65em;
    border-radius: 50%;
    transform: scale(0);
    transition: 120ms ease-in-out;
    box-shadow: inset 1em 1em #3098f8;
    }

    input[type="radio"]:checked::before {
    transform: scale(1);
    }
</style>

# Hello World! 

<section class="top-cards-cards">
    <div class="conteiner-carousel">
        <input type="radio" name="carousel" checked/>
        <input type="radio" name="carousel"/>
        <input type="radio" name="carousel"/>
        <input type="radio" name="carousel"/>
        <input type="radio" name="carousel"/>
        <div id="carousel">
            <div class="carousel-item">
                🔭 I’m currently working on ...
            </div>
            <div class="carousel-item">
                🌱 I’m currently learning ...
            </div>
            <div class="carousel-item">
                👯 I’m looking to collaborate on ...
            </div>
            <div class="carousel-item">
                🤔 I’m looking for help with ...
            </div>
            <div class="carousel-item">
                💬 Ask me about ...
            </div>
        <div>
    </div>
</section>

[![viniciusNoleto's GitHub stats](https://github-readme-stats.vercel.app/api?username=viniciusNoleto)](https://github.com/viniciusNoleto/github-readme-stats)

<div class="social-media">
    <a href="https://www.instagram.com/noletovini/" class="fa fa-instagram"
    target="_blank" rel="noopener noreferrer" style="color:#f0335c;"></a>
</div>
<div class="social-media">
    <a href="https://www.instagram.com/noletovini/" class="fa fa-linkedin"  target="_blank" rel="noopener noreferrer" style="color:#184fa3;"></a>
</div>
