<template>
  <div>
    <NavBar />
    <form-cadastro />
    <button @click="modalCadastro = true">salvar</button>
  </div>
</template>

<script>
import NavBar from './components/NavBar'
import FormCadastro from './components/FormCadastro'

export default {
  name: 'App',
  components:{
    NavBar,
    FormCadastro
  },
  data (){
    return {
     
    }
  },

}
</script>