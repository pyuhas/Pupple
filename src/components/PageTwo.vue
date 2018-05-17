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
        <h1 class="site-header-1">Let's find your new buddy:</h1>
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
            <input placeholder="Name?">
            <input placeholder="Email address?">
            <input placeholder="Age?">
            <input placeholder="# in household?">
            <input placeholder="Children in home?">
            <input placeholder="Rent or own?"></br>
            <input placeholder="Where will dog sleep?">
            <input placeholder="Any allergies?">
            <input placeholder="Willing to train?">
            <input placeholder="Why adopt?">
            <input placeholder="Had pets before?">
            <input placeholder="Occupation?"></br>
            <input placeholder="Daily work schedule?">
            <input placeholder="Typical weekend?">
            <input placeholder="Indoor/Outdoor person?">
            <input placeholder="How active are you?">
            <input placeholder="Travel often?">
            <input placeholder="Any concerns?">
          </template>
        </form>
      </div>

      <div class="submit-button">
        <p>Submit</p>
        <!-- <button @click='getMatches'>Submit</button> -->
      </div>

      <main class="site-content">
        <div class="background-image-2">
          <img src="https://www.billingsk9coaching.com/wp-content/uploads/2018/02/group1.png" style="height:500px; width:1200px" alt="dog-pic">
        </div>
      </main>

      <footer class="site-footer">
        <p>&copy; 2018 Pupple. All Rights Reserved.</p>
      </footer>
    </body>

  </div>
</template>

<!-- when you do fetch, you want it to alter
pass in prop?
populate with the matches -->


<script>

export default {
  name: 'PageTwo',
  props: ['showPage', 'togglePage', 'getMatches'],

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

.submit-button {
  background-color: #51bbd9;
  top: 200px;
  right: 190px;
  /* justify-content: space-around; */
  font-family: Comfortaa;
  font-size: 20px;
  text-align: center;
  position: fixed;
  cursor: url("https://s3-us-west-2.amazonaws.com/s.cdpn.io/9632/happy.png"), auto;
  border-radius: 6px;
  padding: 0px;
  font-size: 20px;
  text-decoration: none;
  border: none;
  color: white;
}

button {
  bottom: 20px;
  right: 680px;
  border-width: 1px;
  justify-content: space-around;
  background-color: grey;
  color: white;
  font-family: Comfortaa;
  font-size: 20px;
  text-align: center;
  position: fixed;
  cursor: wait;
  border-radius: 6px;
  text-decoration: none;
  border: none;
  color: white;
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
margin-top: 15.5%;
margin-left: 8%;
margin-bottom: 5px;
}

#form {
display: flex;
position: fixed;
margin: 70px 160px 120px 150px;
background-color: grey;
padding: 2%;
font-family: Comfortaa;
font-size: 25px;
text-align: center;
flex-direction: column;
width: 75%;
color: white;
border-radius: 25px;
}

#type {
display: flex;
width: 260px;
font-size: 1px;
font-family: Comfortaa;
}

</style>
