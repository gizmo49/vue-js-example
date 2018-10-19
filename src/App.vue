<template>
  <div id="app"> 
  <app-header></app-header>         
    <h1>{{shout()}}</h1>
    <ninja></ninja>   
    <app-footer></app-footer>
  </div>
</template>

<script>
import Ninja from './Ninja.vue';
import Header from './components/header.vue';
import Footer from './components/footer.vue';


export default {
  name: 'app',
  components:{
    'ninja': Ninja,
    'app-header': Header,
    'app-footer': Footer
  },
  data () {
    return {
      msg: ' Vue.js just too awesome '
    }
  },
  methods:{
    shout: function(){

       return "heyyyy";
    }
  }
}
</script>

<style>
h1{
  text-align: center;
}
</style>
  