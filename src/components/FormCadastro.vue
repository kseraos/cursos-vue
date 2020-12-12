<template>
   <b-modal id="modal-1" title="BootstrapVue" v-model="abrirModal">
    <p class="my-4">Hello</p>
  </b-modal>
</template>

<script>
export default {
    nome: 'FormCadastro',
    data (){
        return{

        }
    },
    computed:{
        abrirModal: {
            get() {
                 return this.$store.state.modalCadastro
            },
            set(v){
                this.$store.commit('abrirModalCadastro', v)
            }
          
        }

    }
}
</script>