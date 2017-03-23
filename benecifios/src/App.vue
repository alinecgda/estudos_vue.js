<template>
  <div>
    <MenuBeneficios>
    </MenuBeneficios>
    <div class="beneficios-content text-center">
    <input type="search" class="form-control dark" @input="filtro = $event.target.value" placeholder="Pesquise pelo nome..."> 
    {{filtro}}
      <h1 class="beneficios__title text-center">{{ msg }}</h1>
      <beneficio>
      </beneficio>
    </div>
  </div>
</template>

<script>
import MenuBeneficios from './components/notshared/menu-beneficios/MenuBeneficios.vue';
import Beneficios from './components/notshared/beneficios/Beneficios.vue';
export default {
  components:{
    'MenuBeneficios': MenuBeneficios,
    'beneficio': Beneficios
  },
  data () {
    return {
      msg: 'DESCONTOS EXCLUSIVOS PARA TUDO QUE VOCÊ PRECISA.',
      filtro: ''
    }
  },

  computed:{
    filtroNome(){
      if (this.filtro){
        return;
      }else{
        return this.beneficios;
      }
    }
  }
}
</script>

<style>
  *{
    margin: 0 auto;
  }
  .beneficios-content {
    overflow: auto;
    background: url("http://rebens.com.br/fullpower//application/public/imgs/bg-beneficios.jpg") repeat;
    padding-bottom: 1em;
  }
  .beneficios__title {
    font-family: Helvetica, sans-serif;
    font-size: 2em;
    color: white;
    text-transform: uppercase;
    margin-top: 1em;
    margin-bottom: 1em;
  }
  .form-control.dark {
    border: none;
    background: rgba(0, 0, 0, .3);
    box-shadow: none;
    color: white;
    border-radius: 25px;
    width: 265px;
  }
</style>
