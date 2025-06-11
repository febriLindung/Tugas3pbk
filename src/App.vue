<template>
  <div>
    <h1>Aplikasi Pemesanan Makanan</h1>

    <OrderPage />

    <InfoBox>
      <p> Promo Hari Ini: Gratis es teh manis untuk setiap pesanan!</p>
    </InfoBox>
  </div>
</template>

<script>
import OrderPage from './components/OrderPage.vue'
import InfoBox from './components/InfoBox.vue'

export default {
  name: 'App',
  components: {
    OrderPage,
    InfoBox
  }
}
</script>
