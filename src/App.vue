<template>
  <h1>{{ title }}</h1>
 <Modal header="Sign up for the Giveaway!" />
</template>

<script>
import Modal from './components/Modal.vue'

export default {
  name: 'App',
  components: { Modal },
  data() {    
    return{ 
      title: 'My First Vue App :)'
    }
  }
 /* , methods: {
    handleClick(){
      console.log(this.$refs.name)
      this.$refs.name.classList.add('active')
      this.$refs.name.focus()
    }
  }*/
}
//You should split your apps into different components, to make your project modular and reusable with your different components.
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
h1 {
  border-bottom: 1px solid #ddd;
  display: inline-block;
  padding-bottom:10px;
}
</style>
