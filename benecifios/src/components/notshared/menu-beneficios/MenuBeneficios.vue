<template>
  <nav class="row nav-beneficios">
    <div class="col-md-10 col-md-offset-1">
      <ul class="lista-categorias">
        <li class="lista-categoria-item" v-for="categoria of categorias">
            <categorias :img="categoria.img" :span="categoria.span">
            </categorias>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
import Categorias from '../Categorias/Categorias.vue';
export default {
    components:{
        'categorias': Categorias
    },
    data(){
        return{
            categorias:[
                {
                    img: 'http://rebens.com.br/fullpower/application/public/imgs/food-icon.png',
                    span: 'Alimentação'
                },
                {
                    img: 'http://rebens.com.br/fullpower/application/public/imgs/educacao.png',
                    span: 'Educação'
                },
                {
                    img: 'http://rebens.com.br/fullpower/application/public/imgs/eletro-eletronico.png',
                    span: 'Eletronicos & Eletrodomésticos'
                },
                {
                    img: 'http://rebens.com.br/fullpower/application/public/imgs/entretenimento-e-lazer.png',
                    span: 'Entretenimento & Lazer'
                },
                {
                    img: 'http://rebens.com.br/fullpower/application/public/imgs/lojas-de-departamento.png',
                    span: 'Lojas de departamento e Supermercados'
                },
                {
                    img: 'http://rebens.com.br/fullpower/application/public/imgs/moda.png',
                    span: 'Moda'
                },
                {
                    img: 'http://rebens.com.br/fullpower/application/public/imgs/moveis-decoracao.png',
                    span: 'Móveis & Decoração'
                },
                {
                    img: 'http://rebens.com.br/fullpower/application/public/imgs/saude.png',
                    span: 'Saúde & Beleza'
                },
                {
                    img: 'http://rebens.com.br/fullpower/application/public/imgs/servicos-e-outros.png',
                    span: 'Serviços & Outros'
                },
                {
                    img: 'http://rebens.com.br/fullpower/application/public/imgs/lazer-icon.png',
                    span: 'Viagens & Turismo'
                },
                {
                    img: 'http://rebens.com.br/fullpower/application/public/imgs/todos.png',
                    span: 'Todos'
                }
            ]
        }
    }
}
</script>
    
<style scoped>
    .nav-beneficios {
        text-align: center;
        background-color: #FDD700;
        color: #373737;
        padding: 4px 0;
    }
    .beneficio__icon {
        margin-bottom: 5px;
    }
    .lista-categorias{
        list-style: none;
        display: -webkit-flex;
        align-items: baseline;
    }
    .lista-categorias, .lista-categoria-item{
        display: inline-flex;
        margin: 5px;
    }
    .lista-categoria-item{ 
        width: 100px;  
        min-width: 90px;
    }
</style>
