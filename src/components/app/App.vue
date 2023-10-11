<template>
  <div class="app">
    <div class="content">
      <AppInfio :allSoni="movies.length" :KorilganSoni="movies.filter(f => f.favourite).length"/>
        <!-- movies.filter(f => f.favourite).length bu true bo'lganlar sonisni olib beradi -->
      <div class="search-panel">
        <SearchPanel />
      </div>
      <div class="move-list">
        <MoveList :movies="movies" />
      </div>
    </div>
  </div>
</template>
<script>
import AppInfio from '@/components/app-info/AppInfio.vue'
import SearchPanel from '@/components/search/SearchPanel.vue'
import MoveList from '../move-list/MoveList.vue';
export default {
  components:{
    AppInfio,
    SearchPanel,
    MoveList
},
  data() {
    return {
      movies: [
        {
          name: 'oqibat',
          viewers:5,
          like: true,
          favourite: false
        },
        {
          name: 'Temir xotin',
          like: false,
          viewers: 6,
          favourite: false,
        },
        {
          name: 'Temir xotin w',
          like: false,
          viewers: 9,
          favourite: true,
        },
      ]
    }
  }
}
</script>
<style>

</style>