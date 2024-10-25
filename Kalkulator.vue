<script>
export default {
  data() {
    return {
      bilangan1: 0,
      bilangan2: 0,
      hasil: 0,
    };
  },
  methods: {
    hitung() {
      this.hasil = this.bilangan1 + this.bilangan2;
    },
  },
};
</script>

<template>
<div>
    <h2>Kalkulator Sederhana</h2>
    <input type="number" v-model.number="bilangan1" placeholder="Masukkan Bilangan 1" />
    +
    <input type="number" v-model.number="bilangan2" placeholder="Masukkan Bilangan 2" />
    =
    <input type="number" :value="hasil" readonly />
    <br /><br />
    <button @click="hitung">Hitung</button>
  </div>
</template>

<style scoped>
input {
  margin: 5px;
  width: 100px;
}
button {
  margin-top: 10px;
}
</style>