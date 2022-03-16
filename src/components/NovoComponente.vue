<template>
  <div class="contador">
    <h1>Contador: {{ i }}</h1>
   <button @click="diminuir">-</button><button @click="aumentar">+</button>
  </div>
</template>

<script>
export default {
  name: 'Contador-vue',
  data() {
    return {
      i: 0
    }
  },
  methods: {
    aumentar() {
      this.i++;
    },
    diminuir() {
      this.i--;
    }
  }
}
</script>