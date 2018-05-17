<template>
  <div id="app">
    <PageOne v-if= 'showPage' :showPage='showPage' :togglePage='togglePage' />
    <PageTwo
      v-else= 'showPage'
      :showPage='showPage'
      :togglePage='togglePage'
      :getMatches='getMatches'/>
  </div>
</template>

<script>
  import PageOne from './components/PageOne.vue'
  import PageTwo from './components/PageTwo.vue'

export default {
  name: 'app',
  components: {
    PageOne,
    PageTwo
  },
  data (){
    return {
      showPage: true
    }
  },
  methods: {
    togglePage(){
      if (this.showPage){
        this.showPage=false
      }else{
        this.showPage=true
      }
    },
    getMatches(){
      fetch('http://localhost:3000/animals')
        .then(function(response){
          return response.json();
        })
        .then(function(match){
          console.log(match);
        });
    }
  },


}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
