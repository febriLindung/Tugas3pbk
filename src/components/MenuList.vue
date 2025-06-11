<template>
  <div>
    <h3>Daftar Menu:</h3>
    <FoodItem v-for="(makanan, i) in menu" :key="i" :nama="makanan" @pilih="kirimKeParent"/>
  </div>
</template>

<script>
import FoodItem from './FoodItem.vue';

export default {
  name: "MenuList",
  components: { FoodItem },
  data() {
    return {
      menu: ['Nasi Goreng', 'Ayam Bakar', 'Bakso', 'Sate Ayam']
    };
  },
  methods: {
    kirimKeParent(namaMakanan) {
      this.$emit('makananDipilih', namaMakanan);
    }
  }
}
</script>
