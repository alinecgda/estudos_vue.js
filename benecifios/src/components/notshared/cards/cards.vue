<template>
<div class="companies">
    <cards2  v-for="card of teste" 
        :nomeEmpresa="card.nomeEmpresa" 
        :logoEmpresa="card.logoEmpresa" 
        :desconto="card.desconto" 
        :descricaoDesconto="card.descricaoDesconto"
        :tipoLoja="card.tipoLoja">
    </cards2>   
</div>
</template>

<script>
import Cardes from './cards2.vue';   
export default{ 
    components:{
            'cards2': Cardes
        },
    data(){
        
        return{
            teste:[
                {
                    nomeEmpresa: 'Bristol',
                    logoEmpresa: 'http://www.rebens.com.br/uploads/beneficios/bristol230-01-20151301175359256_150.png',
                    desconto: '10%',
                    descricaoDesconto: 'Desconto: 10% para a nossa melhor tarifa do dia.',
                    tipoLoja: 'http://rebens.com.br/fullpower/application/public/imgs/icon-loja-fisica.png'
                },
                {
                    nomeEmpresa: 'Bristol',
                    logoEmpresa: 'http://www.rebens.com.br/uploads/beneficios/bristol230-01-20151301175359256_150.png',
                    desconto: '10%',
                    descricaoDesconto: 'Desconto: 10% para a nossa melhor tarifa do dia.',
                    tipoLoja: 'http://rebens.com.br/fullpower/application/public/imgs/icon-loja-fisica.png'
                },
                {
                    nomeEmpresa: 'Bristol',
                    logoEmpresa: 'http://www.rebens.com.br/uploads/beneficios/bristol230-01-20151301175359256_150.png',
                    desconto: '10%',
                    descricaoDesconto: 'Desconto: 10% para a nossa melhor tarifa do dia.',
                    tipoLoja: 'http://rebens.com.br/fullpower/application/public/imgs/icon-loja-fisica.png'
                },
                {
                    nomeEmpresa: 'Bristol',
                    logoEmpresa: 'http://www.rebens.com.br/uploads/beneficios/bristol230-01-20151301175359256_150.png',
                    desconto: '10%',
                    descricaoDesconto: 'Desconto: 10% para a nossa melhor tarifa do dia.',
                    tipoLoja: 'http://rebens.com.br/fullpower/application/public/imgs/icon-loja-fisica.png'
                }
            ]
        }
         
    }
   
}
</script>

<style>
    .companies{
        display: flex;
        justify-content: space-around;
        align-items: center;
        flex-wrap: wrap;
        box-sizing: border-box;
        text-align: left;
        max-width: 1200px;
    }
    .card__wrapper {
        align-self: flex-start;
        box-sizing: border-box;
        display: inline-block;
        position: relative;
        min-width: 245px;
        height: 350px;
        padding: 5px;
        margin: 30px 5px;
        font-family: "Arial";
    }
    .company__card {
        background-color: white;
        padding: 20px;  
        position: static;
        max-width: 245px;
        height: auto;
        text-align: center;
        border-radius: 3px;
    }
    .company__logo {
        width: auto;
        height: 100px;
    }
    .company__content {
        color: rgb(10, 65, 121);
    }

    .company__content hr {
        margin: 2px 0;
    }

    .company__card__title {
        text-align: center;
    }
    .company__call {
        display: flex;
        width: 100%;
        height: 60px;
        align-items: center;
        justify-content: center;
    }
    .company__main_text {
        font-size: 60px;
        font-weight: 800;
        font-family: 'Avenir Next';
        margin-bottom: 0px;
    }
</style>