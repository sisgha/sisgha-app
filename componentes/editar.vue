<template>
  <button @click="openModal"><img class="edi" src="~/assets/Editar.png" alt="">  
    <slot></slot>
  </button>
</template>
<script>
export default {
  name: 'editar',
  
  methods: {
    openModal() {
      this.$emit('openModal');
    },
  },
}

</script>
<style>
.edi{
  position: absolute;
  margin-left: 90px;
  margin-top: 4px;/*acres*/
  width: 0px;
}
.edi:hover{
  cursor: pointer;
}
</style>