<template>
  <div>
    <h2>Halaman Pemesanan</h2>
    <MenuList @makananDipilih="tampilkanPesanan" />
    <p><strong>Pesanan Kamu:</strong> {{ pesanan }}</p>
  </div>
</template>

<script>
import MenuList from './MenuList.vue';

export default {
  name: "OrderPage",
  components: { MenuList },
  data() {
    return {
      pesanan: 'Belum ada pesanan'
    }
  },
  methods: {
    tampilkanPesanan(makanan) {
      this.pesanan = makanan;
    }
  }
}
</script>
