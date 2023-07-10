<template>
  <div class="home">
    <div class="cabecera">
      <div class="titulo">
        <h1>Open Music</h1>
      </div>
    </div>
    <div class="categorias">
      <h1>Categorías</h1>
      <div class="btn_container">
        <!-- <button @click="$router.push('/pop')">Pop</button> -->
        <button @click="redirectTo('/pop')">Pop</button>
        <button @click="redirectTo('/rock')">Rock</button>
        <button @click="redirectTo('/rap')">Rap</button>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
//import  from '@/components/'

export default {
  name: 'HomeView',
  components: {},
  methods:{
    redirectTo(ruta){
      this.$router.push(ruta)
    }
  }
}
</script>

<style scoped>
.cabecera{
  border: 1px solid black;
  width: 80%;
  margin: 0 auto;
  padding: 1rem ;
}
.titulo{
  background: rgb(189, 188, 188);
  padding: 2rem ;  
}

.btn_container{
  display: flex;
  width: 50%;
  margin: 0 auto;
  gap: 2px;

}
button{
  flex-grow: 1;
  border: none;
  background: green;
  border-radius: 8px ;
  padding: 13px;
  color:white;
  margin:4px
}
</style>
