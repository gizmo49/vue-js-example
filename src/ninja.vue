<template>
  
    <ul>
      <li  v-for="lad in lads"  v-on:click="lad.show = !lad.show" > 

        <h1>{{lad.name}}</h1> 
        <h3 v-show="lad.show">{{lad.speciality}}</h3>

      </li>
      
    </ul>

</template>

<script>

export default {
  data () {
    return {
      
      lads: [
        {name:'Ryu',speciality:'Vue commponent', show:false},
          {name:'jame',speciality:'Doctor', show:false},
            {name:'dale',speciality:'writer', show:false},
              {name:'mike',speciality:'plumber', show:false},
                {name:'taye',speciality:'tailor', show:false},
                  {name:'muik',speciality:'instructor', show:false}
      ]
    }
  },
  methods:{
    
  }
}
</script>

<style>
</style>
  