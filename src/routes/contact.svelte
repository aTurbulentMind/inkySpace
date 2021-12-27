<body>
    
<h1>Contact Us</h1>
   


<div class="form">
   <h3>Our contact form is the best way to reach us:</h3>
    <form action="https://formsubmit.co/joelkrivers@yahoo.com" method="POST">
     <input type="hidden" name="_subject" value="Hello friend">   
     <p>Artist of choice:</p>
     <input type="radio" id="bonnie" name="pref_artist" value="Bonnie">
     <label for="bonnie">Bonnie</label>
     <br><br>
     <input type="radio" id="css" name="pref_artist" value="Jessie">
     <label for="css">Jessie</label>
     <br><br>
     <input type="radio" id="javascript" name="pref_artist" value="JavaScript">
     <label for="javascript">Other</label> 
     <br><br>
     <p>What's your email:</p>
     <input type="email" name="email" placeholder="Email" required>
     <input type="hidden" name="_next" value="https://tender-benz-1741cd.netlify.app/">
     <br><br>
     <p>Tell us about your tattoo:</p>
     <textarea name="t1" id="plan_for_art" cols="35" rows="5"></textarea>
     <br><br>
     <p>Side note:</p>
     <input type="text" rows=4 cols=20 name="message" placeholder="Allergies or something"  required>
     <br><br>
   <!--  <p>A picture or few can help form an idea for your piece (but is not required):</p>
     <input type="file" class="img-input" onchange="readURL(this)" accept="Image/"/>
     <br><br>-->
     <button type="submit">Submit</button>
    </form>
</div>

    <div class="social">
       <h2>Or you can find us on Facebook</h2>
    <a href="https://www.facebook.com/OATHBremerton/">  <img src="/src/assets/img/fbBanner.png" alt=""></a> 
    </div>


</body>

<style lang="scss"> 
   @import 'components';

   .resizedTextbox {width: 300px; height: 50px}

   .form {
      @include glassBack();
      margin: 13% 13% 25% 13%;
      padding: 10%;
      contain: content;
   }

   h2{
      margin-bottom: 10%;
   }

   h3{
      font-weight: 100;
      font-size: 3.5vh;
      margin-bottom: 15%;
   }

   p{
      margin: 7% 0;
   }

 button{
    background: rgba(16, 15, 17, 0.616);
        outline: none;
        font-weight: 100;
        letter-spacing: 2px;
        border: 1px solid white;
        color: $textColorMain;
        text-transform: uppercase;
        padding: 10px;
        margin:15% 0 10% 0;

        &:hover {
           transition: all 0.2s ease-in-out;
        background: $textColorMain;
        color: $backgroundMain;
        transform: scale(1.05);
        }
 }

 img {
    width: 90%;
    height: 90%;
    margin: 4% 4% 20% 4%;
    border: 1px solid $backgroundSecond;
    border-radius:2%;
 }

</style>