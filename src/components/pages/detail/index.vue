<template>
  <div>
    <h1>This is Detail Page!!</h1>
    <ul>
      <li class="detail-item" v-for="l in list" :key="l.id" @click="move(l.id)">
        <span>{{l.id}} {{l.name}}</span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      list: [
        { id: "001", name: "Aさん" },
        { id: "002", name: "Bさん" },
        { id: "003", name: "Cさん" },
        { id: "004", name: "Dさん" },
        { id: "005", name: "Eさん" },
        { id: "006", name: "Fさん" }
      ]
    };
  },
  methods: {
    move(id) {
      this.$router.push(`/detail/${id}`);
    }
  }
};
</script>

<style>
.detail-item {
  cursor: pointer;
  line-height: 40px;
}
.detail-item > span {
  text-decoration: underline;
}
.detail-item > span:hover {
  opacity: 0.8;
}
</style>
