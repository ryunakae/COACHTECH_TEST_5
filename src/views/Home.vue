<template>
  <div class="home">
    <ul>
      <li>
        <router-link :to="{ name: 'Member', params: { id: 1 } }">
          １へ進む
        </router-link>
      </li>
      <li>
        <router-link :to="{ name: 'Member', params: { id: 2 } }">
          ２へ進む
        </router-link>
      </li>
      <li>
        <router-link :to="{ name: 'Member', params: { id: 3 } }">
          ３へ進む
        </router-link>
      </li>
    </ul>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
  },
  // data () {
  //   return {
  //     id: []
  //   }
  // }
}
</script>

<style scoped>
ul {
  padding: 0;
}
li {
  list-style: none;
}
</style>
