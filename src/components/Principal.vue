<template>
  <main>
    <section class="container text-justify">
      <!-- tercer paso -->
      <Table :dataUsers="personajes"/>
    </section>
  </main>
</template>

<script>
/* primer paso */
import Table from './mainHijos/Table';

export default {
  name: 'Principal',
  data() {
      return {
          personajes: [
            {nombre: "Rick Sanchez", src:"https://rickandmortyapi.com/api/character/avatar/1.jpeg"},
            {nombre: "Morty Smith", src:"https://rickandmortyapi.com/api/character/avatar/2.jpeg"},
            {nombre: "Summer Smith", src:"https://rickandmortyapi.com/api/character/avatar/3.jpeg"},
            {nombre: "Beth Smith", src:"https://rickandmortyapi.com/api/character/avatar/4.jpeg"},
            {nombre: "Jerry Smith", src:"https://rickandmortyapi.com/api/character/avatar/5.jpeg"},
            {nombre: "Abadango Cluster Princess", src:"https://rickandmortyapi.com/api/character/avatar/6.jpeg"},
          ]
      }
  },
  // segundo paso
  components:{
    Table
  }
}
</script>

<style scoped>
   main{
    background-image: url('https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png');
    background-repeat: no-repeat;
    background-size: cover;
    /* height: 100%; */
  }
</style>
