<body>

    <div class="art-banner" id="art-banner">
  <div class="art-banner-bg"></div>
  <div class="banner-text">Welcome</div>
  
  <div class="coaButt2">
    <p><a href="https://www.facebook.com/OATHBremerton/">FB</a></p>
    <p> <a href="https://www.instagram.com/OATHBremerton/">IG</a></p>
  </div>
</div>

    <h1>Things</h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus doloribus corporis quisquam perspiciatis? Expedita dolore unde ullam quisquam, repellat consectetur? Veniam in debitis hic quisquam!</p>

    <div class="icom">
        <a href="/staff"> <h2>Meet Our People</h2>
        <img src="/src/assets/img/purp.png" alt=""></a>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sit, sapiente voluptate. Nobis quae aliquid vitae rerum necessitatibus.</p>
    </div>

    <div class="icom">
        <a href="/story"> <h2>Learn Our Story</h2>
        <img src="/src/assets/img/purp.png" alt=""></a>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Amet atque accusantium at dolorum ipsum incidunt.</p>
    </div>

    
    <h1>Nice Words</h1>
    <h2>This Person</h2>
    <p>"Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus doloribus corporis quisquam perspiciatis? Expedita dolore unde ullam quisquam, repellat consectetur? Veniam in debitis hic quisquam!" &nbsp; &nbsp; &nbsp;  </p>
    
    <h2>That Lady</h2>
    <p style="margin-bottom: 30%;">"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Soluta alias quaerat doloremque! Qui debitis ad similique quibusdam recusandae consequuntur quaerat vitae illo!" &nbsp; &nbsp; &nbsp; </p>
</body>


<style lang="scss">

    @import 'components';

    h1, h2 { 
        font-weight: 400;
    }
    
    


.art-banner {
    height: 100vh;
    display: grid;
    background:$backgroundMain;
    grid-template-columns: 20px 1fr 1fr 1fr 20px;
    grid-template-rows: 20px 1fr 1fr 1fr 20px;
    margin: 5px 0;
    z-index: 99;

    a {
        font-size: 3vw;
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
    background-attachment: fixed;
    background-position: top;
    background-size: 90%;
    opacity: 0.15;
    grid-column: 1 / -1;
    grid-row: 1 / -1;

    img {
        width: 100%;
        padding: 15%;
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
    transform: rotate(7deg);

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

@media (min-width:750px){
    .art-banner-bg {
    background-size: 70%;
}

p {
              margin-left: 15%;
          }
}

@media (min-width:1000px) {
 .art-banner-bg {
    background-size: 50%;
}
      }



</style>