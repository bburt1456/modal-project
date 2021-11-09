<template>
  <h1>{{ title }}</h1>
 <div v-if="showModal">
   <Modal header="Sign up for the Giveaway!"/>
 </div>
</template>

<script>
import Modal from './components/Modal.vue'

export default {
  name: 'App',
  components: { Modal },
  data() {    
    return{ 
      title: 'My First Vue App :)',
      showModal: false
    }
  }
 , methods: {
   toggleModal(){
     this.showModal = !this.showModal
     }
   }
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
