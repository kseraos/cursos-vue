<template>
    <div class="row">
     <div class="col-md-3" v-for="c in cursos" :key="c.url">
        <b-card
            :title="c.nome"
            :img-src="c.capa"
            img-alt="Image"
            img-top
            tag="article"
            style="max-width: 20rem;"
            class="mb-2"
        >
            <b-card-text>
             {{c.url}}
            </b-card-text>

            <b-button href="#" variant="primary">Ver Detalhes</b-button>
        </b-card>
    </div>
    </div>
</template>

<script>
export default {
    nome: 'PainelCursos',
    data(){
        return {
            cursos: [ 
                {
                    nome: 'Curso PHP',
                    url: 'https://curso.php',
                    capa:'https://picsum.photos/600/300/?image=25',
                    descricao: "Curso legal de php"
                },
                {
                   nome: 'Curso JavaScript',
                    url: 'https://curso.javascript',
                    capa:'https://picsum.photos/600/300/?image=25',
                    descricao: "Curso legal de javascript" 
                },
            ]
        }
    }
}
</script>