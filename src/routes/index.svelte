<body>

    <div class="art-banner" id="art-banner">
  <div class="art-banner-bg"></div>
  <div class="banner-text">Welcome</div>
  
  <div class="coaButt2">
    <p><a href="/test">FB</a></p>
    <p> <a href="/test">IG</a></p>
  </div>
</div>

    <h1>Things</h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus doloribus corporis quisquam perspiciatis? Expedita dolore unde ullam quisquam, repellat consectetur? Veniam in debitis hic quisquam!</p>

    <div class="icom">
        <h2>Meet: This Person</h2>
        <img src="/src/assets/img/purp.png" alt="">
    </div>

    <div class="icom">
        <h2>Meet: This Person</h2>
        <img src="/src/assets/img/purp.png" alt="">
    </div>

    
    <h1>Nice Words</h1>
    <h2>This Person</h2>
    <p>"Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus doloribus corporis quisquam perspiciatis? Expedita dolore unde ullam quisquam, repellat consectetur? Veniam in debitis hic quisquam!" &nbsp; &nbsp; &nbsp;  </p>
    
    <h2>That Lady</h2>
    <p>"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Soluta alias quaerat doloremque! Qui debitis ad similique quibusdam recusandae consequuntur quaerat vitae illo!" &nbsp; &nbsp; &nbsp; </p>
</body>


<style lang="scss">

    @import 'components';

    
.art-banner {
    height: 100vh;
    display: grid;
    grid-template-columns: 20px 1fr 1fr 1fr 20px;
    grid-template-rows: 20px 1fr 1fr 1fr 20px;
    margin: 5px 0;
    
    a {
        font-size: 3vh;
    }

    &::before {
    content: "";
    opacity: 0.85;
    border-top: 5px solid $backgroundSecond;
    border-right: 5px solid $backgroundSecond;
    grid-column: 4;
    grid-row: 1 / span 4;
    z-index: 2;
}

    &::after {
    content: "";
    opacity: 0.85;
    border-bottom: 5px solid $backgroundSecond;
    border-left: 5px solid $backgroundSecond;
    grid-column: 2 ;
    grid-row: span  4 / 5;
      z-index: 2;
}


}

.art-banner-bg {
    background-image: url(/src/assets/img/blackLogo.jpg);
    background-repeat: no-repeat;
    background-size: 425px 425px;
    opacity: 0.15;
    grid-column: 1 / -1;
    grid-row: 1 / -1;

    img {
        width: 100%;
    }
}

.banner-text {
    font-size: 10vw;
    font-weight: bold;
    grid-column: 2 / span 2;
    grid-row: 3 /* no need to type one*/;
    align-self: center;
    justify-self: center;
}



.coaButt2 {
    display: grid;
    align-self: center;
    justify-self: center;
    grid-column: 3 / 5;
    grid-row: 4 / 4;
    background-color: $backgroundSecond;
    font-weight: bold;
    width: 20vw;
    height: 15vw;
    border-radius: 50%;
    transform: rotate(15deg);

    p {
    margin:auto;
    font-family: $altFont;
}
}

.icom {
 

    img{
        max-width: 100%;
    }
}

</style>