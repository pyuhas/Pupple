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
          <template v-else></br>
            <input placeholder="Name">
            <input placeholder="Email address">
            <input placeholder="# in household?">
            <input placeholder="Children in home?"></br>
            <input placeholder="Other pets?">
            <input placeholder="Had pets before?">
            <input placeholder="How active are you?">
            <input placeholder="Travel often?">
          </template>
        </form>
      </div>

      <div class="submit-button">
        <button type="button">Submit</button>
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

.back-button, a:hover {
bottom: 2%;
right: 48%;
border-width: 1px;
border-radius: 15px;
justify-content: space-around;
padding: 10px;
background-color: grey;
color: #51bbd9;
font-family: Comfortaa;
font-size: 20px;
text-align: center;
position: fixed;
cursor: wait;
}

.submit-button {
  font-family: Comfortaa;
  margin-top: 15%;
  margin-right: 4%;
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

.background-image-2 {
position: fixed;
z-index: -1;
margin-top: 1%;
margin-left: 8%;
margin-bottom: 5px;
}

#form {
display: flex;
position: fixed;
margin: 70px 160px 120px 150px;
font-family: Comfortaa;
font-size: 30px;
text-align: center;
flex-direction: column;
width: 75%;
}

#type {
display: flex;
width: 260px;
font-size: 20px;
font-family: Comfortaa;
}

</style>
