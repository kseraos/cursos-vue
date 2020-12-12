<template>
    <b-navbar toggleable="lg" type="dark" variant="info">
        <b-navbar-brand href="#">CursoLegais</b-navbar-brand>
         <b-navbar-nav class="ml-auto">
               <b-nav-item @click="modalCadastro">Cadastrar Novo</b-nav-item>
         </b-navbar-nav>
    </b-navbar>
    
</template>

<script>
export default {
    nome: 'NavBar',
    methods:{
        modalCadastro(){
            this.$store.commit('abrirModalCadastro', true)
        }
    }
}
</script>