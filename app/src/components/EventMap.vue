<template>
  <div id="map"></div>
  <!-- Reference: https://developers.google.com/maps/documentation/javascript/reference/map#MapOptions -->
  <GoogleMap
    style="width: 100%; height: 500px"
    :api-key="apiKey"
    :center="center"
    :zoom="4"
  >
    <Marker :options="{ position: center }">
      <!-- ポップアップ画面表示 -->
      <InfoWindow>
        <!-- イベント詳細画面は別コンポーネントでデザイン -->
        <EventDetail></EventDetail>
      </InfoWindow>
    </Marker>
  </GoogleMap>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
import { GoogleMap, Marker, InfoWindow } from 'vue3-google-map';
import EventDetail from '@/components/EventDetail.vue';

export default defineComponent({
  // eslint-disable-next-line vue/no-reserved-component-names
  components: { GoogleMap, Marker, InfoWindow, EventDetail },
  setup() {
    const apiKey = ref(import.meta.env.VITE_GOOGLE_MAP_API_KEY);
    const center = { lat: -25.363, lng: 131.044 }; // TODO: Geocoding API で検索できるようにする

    return { apiKey, center };
  },
});
</script>
