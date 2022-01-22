<template>
  <div>
    <v-app-bar app color="secondary" dark>
      <v-spacer>ONE Equal</v-spacer>
      <v-btn color="error" @click="deleteLocalStorage"> 削除する </v-btn>
    </v-app-bar>
  </div>
</template>

<script>
export default {
  name: "Header",
  methods: {
    deleteLocalStorage() {
      this.$emit("delete-local-storage");
    },
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Playfair+Display:ital@1&display=swap");
.spacer {
  font-family: "Playfair Display", serif;
  font-size: 30px;
}
</style>
