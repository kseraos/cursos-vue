<template>
  <div>
    <NavBar />
    <form-cadastro />
    <div class="container">
       <painel-cursos class="mt-3" />
    </div>
  </div>
</template>

<script>
import NavBar from './components/NavBar'
import FormCadastro from './components/FormCadastro'
import PainelCursos from './components/PainelCursos.vue'

export default {
  name: 'App',
  components:{
    NavBar,
    FormCadastro,
    PainelCursos
  },
  data (){
    return {
     
    }
  },

}
</script>