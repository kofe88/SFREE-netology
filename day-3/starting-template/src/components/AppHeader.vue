<template>
       <nav class="navbar navbar-dark bg-dark">
        <div class="container-fluid">
          <a href="#" class="navbar-brand">Marvel</a>

          
          <form class="d-flex">
            <input class="form-control me-2" 
            type="search" 
            placeholder="Поиск" 
            aria-label="Search"
            v-model="search"
            @input="changeSearch(search)"
            >
            <button class="btn btn-outline-light" 
            type="reset"
            @click="()=>{search=''; changeSearch(search)}">
            Все</button>
          </form>
        </div>
      </nav>
</template>

<script>
    export default {
        name: "AppHeader",
        props: ['changeSearch'],
        data() {
            return {
              search: '',
            }
        },
    }
</script>

<style scoped>

</style>
