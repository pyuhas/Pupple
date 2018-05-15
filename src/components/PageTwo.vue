<template lang="html">
  <div class="PageTwo">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <meta http-equiv="X-UA-Compatible" content="ie=edge">
      <title>New buddy:</title>
      <link rel="stylesheet" type="text/css" href="//fonts.googleapis.com/css?family=Comfortaa" />
    </head>

    <body>
      <header class="site-header">
        <h1 class="site-header-1">Here is your new buddy:</h1>
        <nav class="site-nav--main">

        <div class="back-button">
          <button @click='togglePage'>Back</button>
        </div>

        </nav>
      </header>

      <div id="form">
        <form action="">
          <label for="doggo_type">Please answer these questions about yourself to find your fur-ever friend:</label>
          <template v-if="loginType === 'username'">
            <label>Username</label>
            <input placeholder="Enter your username">
          </template>
          <template v-else>
            <label>Email</label>
            <input placeholder="Enter your email address">
          </template>
        </form>
      </div>

      <main class="site-content">
        <!-- <div id="aDog">
        </div> -->
        <div class="background-image-2">
          <img src="http://southpawpetservices.com/wp-content/uploads/2013/05/group-of-dogs-960x336.jpg" style="height:500px; width:1200px" alt="dog-pic">
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
  name: 'PageTwo',
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

/* .site-content {
bottom: 0;
width: 100%;
} */

/* .phone-image {
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

.to-button {
  bottom: 120px;
  right: 667px;
  border-width: 1px;
  justify-content: space-around;
  background-color: grey;
  color: #51bbd9;
  font-family: Comfortaa;
  font-size: 20px;
  text-align: center;
  position: fixed;
  cursor: wait;
  background-color: #bbb;
  padding: .5em;
  border-radius: 6px;
  /* color: #fff; */
  /* font-size: 20px;
  text-decoration: none;
  border: none;
} */

.back-button, a:visited {
bottom: 162px;
right: 40%;
border-width: 1px;
border-radius: 25px;
justify-content: space-around;
padding: 20px;
background-color: grey;
color: #51bbd9;
font-family: Comfortaa;
font-size: 20px;
text-align: center;
position: fixed;
cursor: wait;
}

/* .tagline {
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
} */

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

.background-image-2 {
position: absolute;
z-index: -1;
margin-top: 14%;
margin-left: 8%;
margin-bottom: 5px;
}

#form {
display: flex;
position: fixed;
margin: 150px 20px 20px 250px;
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

/* #aDog {
text-align: center;
margin: 5px 20px 5px 20px;
font-family: Comfortaa;
font-size: 30px;
} */

</style>
