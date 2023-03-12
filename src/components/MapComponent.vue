<!-- <template>
<div class="root">
    <section class="section">
        <h1>Карта с рандомной меткой</h1>
        <div ref="mapContainer"></div>
</section>
</div>
  </template>
  
  <script>
    import L from 'leaflet';
  
    export default {
      name: 'MapComponent',
      mounted() {
        // создаем карту
        const map = L.map(this.$refs.mapContainer).setView([51.505, -0.09], 13);
  
        // добавляем тайлы OpenStreetMap
        L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
          attribution: 'Map data © <a href="https://openstreetmap.org">OpenStreetMap</a> contributors'
        }).addTo(map);
  
        // создаем случайную метку
        L.marker([51.5, -0.09]).addTo(map);
      }
    }
  </script>

<style scoped lang="scss">
.section {
    min-height: 30vh;
  
    .leaflet-container {
      width: 100%;
      height: 100%;
    }
  }

</style> -->