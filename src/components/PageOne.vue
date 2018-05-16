<template lang="html">
  <div class="PageOne">
    <head>
      <meta charset="utf-8">
      <title>Adopt a dog!</title>
      <link rel="stylesheet" type="text/css" href="//fonts.googleapis.com/css?family=Comfortaa" />
    </head>
    <body>
      <header class="site-header">
        <h1 class="site-header-1">Pupple</h1>
      </header>

      <div class="phone-image">
        <img src="https://3.bp.blogspot.com/-XrJcgDnbYl4/WvW7DRLu1gI/AAAAAAAAAcU/Yg_frYTfUG0I5iuEx0oX2Gfm3IysKCfhACK4BGAYYCw/s1600/iphone-hand-mockup-free-1000x640.jpg" style="height:auto; width:2000px" alt="phone">
      </div>

      <main id="main1" class="site-content">
        <div class="benton-image">
          <img src="https://2.bp.blogspot.com/-ZFTdWR3La8U/WvR-ixu0gnI/AAAAAAAAAbs/gTQkAjqxRzopo7XM3Pok-40EXdXfJwLJQCK4BGAYYCw/s1600/Screen%2BShot%2B2018-05-07%2Bat%2B3.34.59%2BPM.png" style="height:400px;width:auto" alt="cute-dog">
        </div>

        <div class="tagline">
          <p>Pupple: Matching Puppies & People</p>
        </div>

        <div class="to-button">
          <button @click='togglePage'>Find my match!</button>
        </div>

      </main>

      <footer class="site-footer">
        <p>&copy; 2018 Pupple. All Rights Reserved.</p>
      </footer>

    </body>

  </div>
</template>




<script>

export default {
  name: 'PageOne',
  props: ['showPage', 'togglePage']
}
</script>




<style scoped>
body {
display: flex;
flex-direction: column;
height: 100%;
width: 100%;
}

.site-header {
display: flex;
margin: -130px 20px 0px -30px;
flex-direction: column;
text-align: center;
justify-content: space-around;
width: 100%;
font-family: Comfortaa;
font-size: 50px;
color: #51bbd9;
position: fixed;
z-index: 40;
}

.site-content {
bottom: 0;
width: 100%;
}

.phone-image {
background-position: center;
display: block;
margin: -200px 20px 0px -220px;
position: fixed;
z-index: -1px;
top: 0%;
}

.benton-image {
display: block;
margin: 70px 5px 75px 550px;
position: fixed;
z-index: 2;
}

button {
  bottom: 150px;
  right: 650px;
  border-width: 1px;
  justify-content: space-around;
  background-color: grey;
  color: white;
  font-family: Comfortaa;
  font-size: 20px;
  text-align: center;
  position: fixed;
  cursor: wait;
  padding: .5em;
  border-radius: 6px;
  font-size: 20px;
  text-decoration: none;
  border: none;
}

.tagline {
font-family: Comfortaa;
position: fixed;
border-style: hidden;
border-width: 1px;
display: flex;
flex-direction: column;
font-size: 20px;
text-align: center;
margin-left: -35px;
bottom: 24%;
width: 100%;
}

.site-footer {
position: fixed;
border-style: hidden;
border-width: 1px;
display: flex;
flex-direction: column;
font-family: Comfortaa;
font-size: 10px;
text-align: center;
bottom: 0%;
margin-left: 0;
width: 15%;
}

/* #form {
display: flex;
position: fixed;
margin: 150px 20px 20px 550px;
justify-content: center;
font-family: Comfortaa;
font-size: 40px;
text-align: center;
flex-direction: column;
}

#type {
display: flex;
width: 260px;
font-size: 20px;
font-family: Comfortaa;
}

#aDog {
text-align: center;
margin: 5px 20px 5px 20px;
font-family: Comfortaa;
font-size: 30px;
} */
</style>
