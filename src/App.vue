<template>
  <div></div>
</template>

<script>
import fly from 'flyio'

export default {
  mounted: function() {
    this.call()
  },
  methods: {
    call(){
      console.log('++++')
      fly.get('/repos/pdk/sxf/docs/pto7d2?raw=1').then((res)=>{
        console.log(res)
      })
    }
  }
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
