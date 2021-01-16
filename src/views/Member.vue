<template>
  <div class="member">
    {{ id }}
    <div>
    <router-link :to="{ name: 'Member', params: { id: this.id - 1 } }">
        前へ
    </router-link>
    <router-link :to="{ name: 'Member', params: { id: this.id + 1 } }">
        次へ
    </router-link>
    </div>
  </div>
</template>

<script>

  export default {
    name: "Member",
    props: ["id"],
  }
</script>