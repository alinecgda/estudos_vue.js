<template>
    <div class="col-md-offset-1 col-md-10">
        <card>
        </card>
        <div class="veja-mais-beneficios">
            <img src="http://rebens.com.br/fullpower/application/public/imgs/seta-ver-mais.png" alt="Veja mais"> 
            Veja mais
        </div>
    </div>
</template>

<script>
import Cards from '../cards/cards.vue';

export default{
    components:{
        'card': Cards
    }
}
</script>

<style scoped>
    .veja-mais-beneficios {
        display: inline-block;
        cursor: pointer;
        transition: all;
        margin-top: 1em;
        color: white;
    }
</style>