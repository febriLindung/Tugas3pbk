<template>
  <div class="food-item">
    <button @click="pilihMakanan">{{ nama }}</button>
  </div>
</template>

<script>
export default {
  name: "FoodItem",
  props: ['nama'],
  methods: {
    pilihMakanan() {
      this.$emit('pilih', this.nama);
    }
  }
}
</script>
