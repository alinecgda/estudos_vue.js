<template>
    <div class="card__wrapper"> 
        <section class="company__card">
            <div class="company__content">
                <div class="company__card__title">
                    <span>{{ nomeEmpresa }}</span>
                </div>
                <hr>
                <div>
                    <img class="company__logo" :src="logoEmpresa">
                    <p class="company__main_text">{{ desconto }}</p>
                    <p class="company__call">{{ descricaoDesconto }}</p>
                </div>
                <div class="company__card__footer">
                    <img :src="tipoLoja" class="store__icon">
                </div>
            </div>
        </section>
    </div>
</template>

<script>
export default{
    props: ['nomeEmpresa', 'logoEmpresa', 'desconto', 'descricaoDesconto', 'tipoLoja'],
    data(){
        return{
           
        }
    }
}
</script>

<style>
    .card__wrapper {
        align-self: flex-start;
        box-sizing: border-box;
        display: inline-block;
        position: relative;
        min-width: 245px;
        height: 350px;
        padding: 5px;
        margin: 30px 5px;
        display: flex;
        justify-content: space-around;
        align-items: center;
        flex-wrap: wrap;
        box-sizing: border-box;
        text-align: left;
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