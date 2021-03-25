<template>
  <section>
    <h1>👍 Compre ou Venda 👎</h1>
    <ProdutosBuscar/>
    <ProdutosListar/>
  </section>
</template>

<script>
import ProdutosBuscar from "@/components/ProdutosBuscar.vue"
import ProdutosListar from "@/components/ProdutosListar.vue"

export default {
  name: 'Home',
  components:{
    ProdutosBuscar, 
    ProdutosListar
  }
}
</script>

<style lang="scss" scoped>
  h1{
    font-size: 2rem;
    color: #87f;
    margin-top: 40px;
    text-align: center;
  }
</style>